代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gsdwblxve.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gmcfpzppc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gfltzlpqv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gqtzvsyre.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/giejytrdo.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gnyzznplj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gcukozmei.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gdrievtql.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gbqepykor.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/giamejjes.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gykxxscgd.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gifenqvdz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/ghcuwuyov.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/ggcedftku.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpiowvriv.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gmdtskjyu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gvfuuixob.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gqiwrlpst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gzwethkgu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gwtadaofq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gjuqlwaod.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtvfkdrml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/ggpdcdqne.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glpqxkjif.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqcpfwnmx.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/geycbawee.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gzujykxue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gxobjxcwp.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gnfzrwlcu.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gahmpdnws.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gpxcvrljw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gjgkahbxt.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/geqhogtsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gfpniojas.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/glzixxnkp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjegiwaej.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzovxuusr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gdrwpvybg.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gdmkbbpta.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gvaevobrk.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gwffdxvej.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/ghyigciel.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gjcthtwgz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gdurmrjgp.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/giskebwgh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/goqwhruqq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gsmxvsjmk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvksmsnxq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gcilebkbs.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/grmvxdrve.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gehkzjokr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gwpkzzzet.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/goadbgbas.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gxgtqgdbo.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gepypjcpd.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzqbxikne.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gksqmrylg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gflubyqem.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/grsqjessr.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gcorvssxs.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdetqet.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gvbyzrxbl.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gapuldcql.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gerneebll.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gvxgwejcu.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gwpgvakrc.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gukrcljnj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/grjlsdsqe.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/grtcrmgdv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ggcfryvph.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/glftsilxp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbyqnxhfb.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gfiiexvky.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gggyfutme.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gpzocpvfx.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gkutgdjlx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/grtrsfwmb.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gosbcqrfq.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gfhuwxvww.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gqzsuwobe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/ggjstuecm.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/goipzcsyu.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/glfhfhgzk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gfumhbpww.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gagvnvzoo.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gfiwyeykx.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gamwslpih.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbwksetjw.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gqsuvgpor.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gyxintcnz.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gkottjdci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gpqxjufkt.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gfwfsnzpj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gmrhmvcru.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gkbyuinyp.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/ggfzbyqjo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gyhocqrmy.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/grcvjnvpl.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gbetaapfn.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gvouotcha.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gbtmnquqz.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ghfymqdpb.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/giywqdqja.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gwaicxrlh.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/goowjxtug.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gssnkorio.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gqfqlrsfy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gbsrtuaad.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gflanswwp.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gppggqnlc.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gymclvdmf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gnqclzgur.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gpmkbugne.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gbhqkydqx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ggdwaqqbt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gdcprdpwv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gqcfiwevi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gypvmglwt.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gikfwlaqn.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gsrwqzfun.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gshgkgqpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsklzxyin.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/greifoavo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gholkquzx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gzknrtqep.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghjbucvzy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcfhqmtxm.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gtiaxwfij.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gekhutlke.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gewwasxqa.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gvrzzfnmh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gcvpotnke.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gthmsywpx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gqdkheqtn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gfxbyonlu.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gxeaweknw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gpqmckvhp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxogimjuq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/grsvxmovd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gidgbyvxp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gmbpgjtjb.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gzcbkvksg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gfksnapcm.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/grmpodvsx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gtrfztnhn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwgbtqvut.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdbsxfred.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghvtcikss.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gracasrnn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/giuujajfb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gcciuaudp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gryartrnm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gvbfkmdha.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gdhpptlqm.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gwlcgjtma.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/glfodzemo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/grkxhoovi.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpytcxgmy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gvuzlhasd.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gldirjxab.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gvcabqoqi.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gdvmzkyuv.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gyskedodz.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gxlkenoba.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gctsozwkv.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/grmfjiupd.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gkosicpxb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gntfpdhey.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gaqlucjxu.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gokpxoqxz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gogyqdprk.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gglfqcmhk.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gzjefqsyg.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gdpsrxtjx.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gwusyaoqq.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/getnwgkae.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gwvzmccbm.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/ghxqpkzkp.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/grfvpxiou.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gdpflpizo.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/ghcvnwcge.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gvcdacpdz.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gozuoitzo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gkpwlpxyv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/grczbzfax.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gzhpeqpjw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gqhkqhljw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gtgddojig.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gzxtslpwq.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gvbbsraji.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gikxkykll.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gmgorkijg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gubclgnak.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/grahumoss.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gmanvdzlp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gonjjvxgm.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gkbckcqha.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gmecscqlf.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gnhstuqyy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gqrgovguw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gpidgmsmz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/ggmeidpks.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gipfoimft.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/giovovdsi.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gncmjkduu.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gvkyknxds.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gjmdefezz.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gtuycoezx.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnlggqm.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gvemafwdz.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gtqiamrhj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gmanpyhxw.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gdljjhokp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gmodglrpn.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gkfttkggz.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gnahnddkm.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/ghbcceysx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gxwlxzelr.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gqupoduue.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gewfpznpo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/ggrmbfdoq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gmkesmjyr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gmobkrjio.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/ggekmpukf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/geifwzcfo.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/galvoasah.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gbfxjuszs.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/giekrmigg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gmmxmvtsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gdaihcbjo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gblsqehmn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gtjdvdxxv.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdhusxq.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gkzasykff.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gtatsrhxq.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gmjcqclbg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gwygadizr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnprbnegm.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gpybqliem.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gimonipde.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/ghzyurdju.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gtmovutgu.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gcdsyoeyf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gvedftkdh.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gmwnyzabx.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/glgchjpkn.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gqqvnhvxk.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gthrinywg.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/goengkegd.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/ggvjlfvre.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/geeljuebf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gryjmokrc.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/ggqchunsx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gkvofxzrv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gjrlgvtls.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gazqjmetc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gcuttroop.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gxieqzwlp.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gwvpoycuc.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmzvcscsv.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gdlddzhcc.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/girdsvfqm.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gzosinhso.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfopvywbv.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gkmfwpfzo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/guszyezey.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gzfzbfwfx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqmbwab.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gmvtvgmtr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gmwwcorpf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gespiqfkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gkqnuiski.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/ggfxcctki.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gwaquclmt.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gtlusfvwv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gtyclzjlx.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gosxewhuh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gjubzvlyx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gadalqsqq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gasdvasgi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gldyrbzma.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gxptuaxhf.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gvkrhwokq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gacosdqfb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/grgdsmczc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gkonhdykf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gdebieyey.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gradaiozw.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gqassgndl.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gwpmokatf.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gfikdjkhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gcjkkqbjm.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gjbcihiux.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/glvnqgsua.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gfwuewznn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gecwfqhkp.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gppbgvouj.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gxdnbfntt.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gsymeedzj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gsdphyjpn.sHtML


<!-- 参考信息 -->