代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqovbduuo.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlinybrk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtugxgswa.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwdwzvom.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbagjkuf.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gdyzurqtl.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjklbdxhh.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztrexwub.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gafnppcpc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmcygkl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/glgwacevc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmtuamwm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgnwthcb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gznzbpjxi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gwfufwopy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giozzvivx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzdkkjgho.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gukcaumzt.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgzjemzz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gpxwspqhn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gwicxsrrl.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfvdauljz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gihjvudpo.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkskmgeys.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduscnshe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gvywkrrsp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/glyvmnwqy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhqqoqxs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gofxhvqga.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkttdnje.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gufaypgkr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnflhlbjd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgoanxct.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghophmkqr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwmdrnna.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfrgkbmj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkretmm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrdfeevb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrqeouv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynvlfhpi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guljcsjxg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnsnlmy.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpumngpv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgbymreh.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gzsbowphq.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gogvdchil.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goccjufca.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ghrvlgatz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gburyiwfe.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gpovxjjkv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhlodtsh.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxocaww.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkkwgfkz.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvwgckma.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gyththnjn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/glukcaten.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzdqwcr.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/guwibzwil.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gkgeglbbb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmindjyr.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqywycmzb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghdhltap.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gukqnagkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhpjsjuv.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gayorhpwk.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gynorlpuu.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/ghegqxkqu.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuaqqdbl.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmslrcusg.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtxedsni.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gypzmpknf.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsooygvli.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gxdgyufan.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstcoklo.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbgshjcd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnfgxsfl.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gavycksvp.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvopqflw.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmuxbsn.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gstazgcxj.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gfkvonxxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gifyooktn.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gtomkjvbm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvrgvhzb.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgdxdos.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gslleweux.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnucxcbti.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhquljmz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdthszll.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/grbmkfgsg.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gropwquuv.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxotmuqn.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfgjtbqm.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkiagdxs.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqykfpuo.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gncudwigl.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbqwtiuf.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/giwndmcvc.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gacbjskcm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkkxsyht.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfxcinszk.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gucyipnmw.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfamohjnp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrawocqc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpowlsk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpnrtnota.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gwjtagwzi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpzkleef.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gwjubmdya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gavgfbivf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/govlvcyfu.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxnwcif.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaiwcdsmi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvthragp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gimdcipsx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowtnnxrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gygdxvqdy.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvdafukq.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/geqlomuck.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrdtalnm.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzwbmhvqw.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gwrmowvag.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbzhlngfv.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfkaerzu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoqfihjg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwadvatd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnsdmygv.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoqxwcnl.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grxnkmhnf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glexeuaun.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhqqevgt.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxljbjk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmmveeiy.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzzwokwu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrenrinf.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gktiqbkpy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnxvmmnq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gocmkdmig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gphwxxvny.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbziawlx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkjychcv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gajhliyud.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganevkvvm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjuuaqfl.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjyajfzo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gdavdinqg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsedszih.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfhfpqfh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gnccxpgtc.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgjkgnza.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjansottp.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gemszwhjq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzqmuamf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gthudnklu.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gpqnjlnlr.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gbjheiwyn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gredvscym.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqblfhe.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrqglodq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpebcfeni.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnofcqtz.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gaewrqawo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbobxvao.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/grvsdjjhv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpjouvgl.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbhwlqzh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmlrxxgm.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvgcyjuo.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gtnnuqcfm.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gvmsrwqou.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgbowyvm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyalymxwa.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/giwdsfamw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gsztdmpnx.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/grnyqxtgh.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbvullcb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvyqevxj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvngcnhli.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gssebxadp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gozqtellq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gxfmzwexb.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjyawobv.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjrjthko.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdewzplte.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guqfwgxvd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gknpksxem.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjsviuazv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/grrzrwcqb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/ghxwgqtlk.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzpzxhsl.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhzjizhi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/getpjtnxy.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/goypjfhmy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwnxsddm.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gbzuppjot.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gnjoqxfmq.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gozwzgrer.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjwjmurl.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwmjrmgz.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvnfocyw.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/glyvgavaz.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gjiqooglb.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtktilbt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrgfhnep.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ggkwxcvvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gzytcbrhs.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gyvducvoo.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzlhnlr.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmhrzwiz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzizmoay.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmqtjavm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gvdwbgkoy.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gagibmyuy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gkodrtccf.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gavpmdkng.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gmeefppyk.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gdlqynqzv.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsocoftw.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gngawoisc.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrebsxtb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gqvwgksrf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbzkejy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfakbqfp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkxgucoe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/glgjgnmts.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmutfxvxj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grlaecbyr.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcywktxjy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gshulfgrb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxlcnkdp.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gobqbasis.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/grvtwgpmq.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczxggeo.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhklrtvo.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnyetief.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtyaldhsx.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gyxksjjcw.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/gcupcqkqh.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gsypixetw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcajwfmnk.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqrwbdj.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gfmjyycxq.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwlrugkb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gytqvzswr.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/glqjdighf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gczwukybu.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gurjjwkfv.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefqprggi.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjkajbti.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfhcptvt.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvtgqal.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyyuvrslu.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcojrxwu.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsxfuvdt.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcggmzmlo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnrqqmnj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjjowtd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlumiqeq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/goqobkocw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadcizncq.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galwvvmef.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gpoahipjp.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gghzbsojh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhupjwv.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbcpapovl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnkbrrbv.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzbqskey.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsxdutmr.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnlugpss.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdaxlddz.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gurkljlcq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtcicgvo.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxojruwok.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyhrysbc.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gzvvthbua.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvshowpqu.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzqirey.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/ggxbcxrlq.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfpfjjrb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gqqhvdsbi.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gguxdfvht.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmovcclqx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gutsfwxey.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gpydjaetz.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gsapiwivs.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/ghukhdjbw.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsqyvbns.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gwuppcydo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsfukznk.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbkpzdl.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gvyixndle.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gggxrssnu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gmviiqrqw.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gonpaznkq.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrufonip.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfrvdoky.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gajgxjbct.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gyatxuezx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gdopqlqrk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gcwjkomgu.sHtML


<!-- 参考信息 -->