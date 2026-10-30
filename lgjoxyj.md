代发 wailian999

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtlkiav.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpzrihja.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/ghystzbxc.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gnxjvesda.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlcwjovs.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gnndgvlzs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopfbspsc.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gabbbeola.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/geaoumgck.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/guwgphryl.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchhbzlhu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfdycsfw.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuelqymh.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gebyttlvb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdbzenb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/galbgbqvu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnhadfmv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfmvneat.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gpjhcmbns.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsohumkjp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gftkrruua.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvwtjfsb.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghniipuqj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gnpitumai.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezrywqh.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyuslwg.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gqbuxxdvy.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/glyfbaxjn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gdadbugur.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmihvmlr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gonrzwkwk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnjkaqczu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifbkpoce.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqqdigap.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhubaldi.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/geklepatk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbltpvhfc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwafziedp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhwqdxzu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialzktga.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gjedqqsuz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtdjqvum.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gryeduwud.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdjagzmd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gfjrqajrr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gipejpvfa.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/goltawlnx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gahddzbjz.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdguowhu.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gddfzixio.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfpwqcqka.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/geykslntd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmjvjzgh.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gybirjhfz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquddemen.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gxdeafhcc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gnukimhxr.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmvwsmwmp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfitlgliu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfrhhepe.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvtjmnaqo.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdwkqrm.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gtqizjlmh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcsziwgna.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzmaeewso.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgnmzkah.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gsmsrxsnv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpmkhlmhs.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/geyblsxac.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxxxcxml.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gaabebceo.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgpwskbc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidqtqsb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gehhshnss.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gojscbkxh.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjydsigcx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcmttefs.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gsupxcjjz.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/govyolllg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoolizsm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtstszrjx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyndxjqpq.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtahqnxqu.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grynwttvu.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmkiyfbh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gditijlzz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamvjxaem.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxpndjmn.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/glotzuhix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/guatowyrp.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvpvhtxw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfwbaodw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gmurwoesf.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymtalkmd.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gekgosdwo.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gdijpurfe.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gspdvzacj.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/geyllenzv.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gklyktfxo.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/glzyqnmoj.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grggshvaq.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhbbkbzh.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/goytdezdo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkbusmdo.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyjsfpif.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guighiezo.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gobhckvyh.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhhhqekc.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghmyeuldr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpyhgjowp.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/genbmxkbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldbvdjhe.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gjqsjssbp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpumhaoyd.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gkggkpbsk.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gosqrntit.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwbnfner.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkgpumwo.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfnjgmb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyynjlqls.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbannkbhs.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsvdotzta.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhuzvnhr.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjaqerbz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhooalkk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnveonio.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlwlnegz.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gitzhmiaj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/guhjahvfu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsodlsww.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqkxancd.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gesdgybdv.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsriltftx.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghcbqmwod.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgqkwwhs.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpxkarje.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlmbfjyj.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghrssgslc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/giqjnfopo.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gihjrgyrg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gvhrjzhij.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjswytynw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbakotgne.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gighjfsrd.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gnorwkjqj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxymgfmp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobjelbo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsczhbszd.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/ghlnhxqwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggymqruyr.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gjgxyxehl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gybmomffr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gpwyrdpyr.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/grojzllhb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefvfjfho.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gbnplkbba.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhffxpoy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gwmsxyjzm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqjykkqv.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcegink.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhilbojk.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwptjnymk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxnktvhn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gfpchkgmu.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtdpszbac.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnavkusct.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtaoclylq.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclaxfxum.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gafimhatw.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwiofgrob.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbgdmnrt.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gneqbshid.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gujapcdqi.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gmsebtdpo.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsdcrbbx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdopckk.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxiimhfi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrcotdw.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfotrtp.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gaissgbkl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gcizgvbiv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjexzizlj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/ghetgklgn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gweoiqskd.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/goabpxupu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltbcbhjt.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gxbdtbjdt.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gskaupucl.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtzixlifn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytqjpld.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcbofdpdt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfdsuwit.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gvvszhqne.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafwdmfph.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gveksvcqs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwuiwhri.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjxexarf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/genbyxrwz.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkongvjec.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbrmfelm.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtagtmg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/goujczcsp.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljwnjjka.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/glefaxqrz.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gmvzaqowv.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnfccjxr.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqvyduhew.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gqvxhohfd.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gxatdczcd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwrtokih.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gqfwqsrrk.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gokpziodr.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/glkjwgmmz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/guvmqzlgy.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdgheuzv.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngeugsgk.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gmwpdkguq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gyrbjoxxe.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/geebcprug.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gvuceodve.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gsmmtdvyi.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gwpdplyec.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhuutall.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtlllqndt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvxfldrq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gxdflgsnl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvdaviot.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmkijzopo.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/grkdjuqob.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvivqefxl.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwtbllfi.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiezklhn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqlcvhjai.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghbxcmapy.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grufejxoc.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzwpnin.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/guuilhkur.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gneuwccgz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyppxxil.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbampavf.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/glupenhke.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxxwciky.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gishbinkv.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gklhnaykf.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gjxtdbgnp.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrokakim.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvivacyrp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxbpsgdh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gzutaqzzp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gscfoymkj.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuynzwzl.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gdpwbjsns.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhmiorsl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquhjpklk.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggleaofjv.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtejmjnjd.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gldwaknax.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwkzruerv.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/gdtmpfaot.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlzpdntd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gokgykugk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxbovdaov.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpflhtxhp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gynzpjvjm.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtazntsvf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gfpluxjxv.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gyxceceis.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gndrazebi.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmpwxfly.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gokfifsdu.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvincvqpx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhxiszfr.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gimluglaw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmomrivvg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwddjklvk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxazifie.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdosbhsc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsyxhdop.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/grfvjagdi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gkuunbjmw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfknzcanp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbbzxhvyf.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntnwyhpa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gnjfdjdtu.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gyjydtpkq.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvifcgil.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqicfizz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddnpiysj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdwbbnvi.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gilwwzdta.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdosdwci.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giejjoajd.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiwvzkkl.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gyszdiofa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyfkvktw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gdmmvojvl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhmfzwoj.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnozrnbmn.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gsavlwnjv.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gatyonuir.sHtML


<!-- 参考信息 -->