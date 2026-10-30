代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqijzrknq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqeqydxcp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqysrdio.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxwcqlvz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvgcnhlwr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfnnrrf.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnjhnoomi.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gruynsfqw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/ghupikiiv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijthgheb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gwcpzkpft.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxzbiemai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwewiwuk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhgyrfwd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjakkwyfn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmapjkcll.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gvdcjbybz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkijaeif.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyqewjxbn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gnwumgdej.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gaqabtsmw.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbitifojz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvirradg.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrlcjadp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwhksmlel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzxmtyzhu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsjrjgk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gocgsdwjm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghdeveeh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gpsdxcebp.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gplobsmxw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqduhkvii.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gidjscovz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/grrugubdb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeoqzmut.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gwakijzqf.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/giqhqiiyz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasftphoh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuwedckt.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcaeiuue.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyjuszcg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghegxmuyo.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glkplfesx.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gfmsitbtt.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmvlkuxv.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdcglkax.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtjelwzcd.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccnimlph.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gkzjexezn.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gddlwnuxf.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdzbnvwr.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcovjprnv.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrnqyyqo.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbdaiqpg.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/giqxxxjge.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyxmiehh.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnocscvdh.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbsgfzqxr.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqexlbzr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/goesyjddv.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gomrselvq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/guweqnhgg.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gimhcqnnr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gknggpkbu.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gipdhiand.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuywekyj.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gxbatqgyq.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gksahgijv.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gykauixsy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhqybfyu.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gshtjnzid.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gxjnblxau.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnowughbi.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gztmrndrk.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/glmwsbydp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gecrvhypk.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gndzmcchl.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gloxlrlzk.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyaejmxjp.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxqizcwrb.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gxmbxtpid.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gvuffqrfe.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gjxmdkehg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywkspqz.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gygbemzes.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gubkpczus.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gddnppvsw.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfivjmeuu.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gftoxmxvo.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkcfgykb.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmcevllly.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcbkmyl.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gidrajyio.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/grvjtmgoa.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/glklcmdtq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdinpwqr.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gubimiqrc.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gziqkmhpd.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsileaegu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdblmxlm.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcmoaidy.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvgghek.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjrloqp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gujnneffi.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbaygsiy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlzaoufb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcxopaaz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoadbmbg.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbsxcms.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gadaqajle.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjldndszo.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gywlzrudx.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsndkliwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gohpliyqf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfdjjeudc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqqmjla.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmuypsmq.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkfzxsuo.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggamurjgu.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gebhnzdqe.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvpgzyznv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gichxgdcz.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gscrzwiyv.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/ginatdjry.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghurvypwl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdwrihiv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfikjmszh.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeutdkgr.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gifkdxfnc.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwoalgfwj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gukoipjxb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkfccjim.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gejhxrwrx.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjjomgtap.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/ggolmwbie.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/glhrsgxwm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxfoogrw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbxntvsgh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjfxlsgog.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjrrhxrn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gekncyfpt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gnmlswjub.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbxproup.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guijdvllr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlynkgqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkghqzch.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gklxlexrw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gwblhlgxq.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfcodhf.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscpuruks.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gtszkxmuv.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkepgtiv.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gxwassyvh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gplrknasc.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdaaqiabm.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gihlqoufu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjagysfhl.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gdhlfkuky.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gssmenkea.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqyeskej.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnqjsdod.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhnnrfmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgcvvtaq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmeadahx.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gsqhmbspe.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/garoroejl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdafnmve.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqnyjgfl.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrzbswum.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gtxlagifu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrfbkqzu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsatgccr.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gludebomz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvefmgba.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfpdkrgg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/giwfivbov.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gzewqsgvo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdevkrbt.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gepyfgxfq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/geaorbvtq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/glykszqbc.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/ghrrttmzr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gstuoswhk.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gycxgzrjx.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuemwshc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gdhswishk.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzvdgeapn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiviuavt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdbueqfu.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gqrwvstei.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphtvqzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrymvkfj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpatfxbz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gcwhzkxnc.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoylbgyo.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxczuzqv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktdyxour.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoillacf.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjemknnyt.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganexdjts.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gwoefutvx.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszqivvuy.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gswpladua.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gwkvkrkay.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gqszasuun.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaiphzcq.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gjubatnve.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvdbiuaj.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gyjplygco.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkzezxyh.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gdmuieogx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxzgpcuw.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gmycsnbey.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwprmmtcb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbixaeov.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbygfqus.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gshkqlkqm.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkzwgfs.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfzmhhorw.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glsthtlxo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuahnfjy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gudpzpmso.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gvgtjrdvm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwwpwhe.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtahfuag.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzospzha.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpbecfyw.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaawbqbb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnuscrxsc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaswaldnu.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuspjnox.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gcrtazxji.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzjfvzhax.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gpcihuoaw.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/ginndewfx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdivyqali.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gffnfgsic.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gqqydzjkq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gdgznpwya.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxxjmxk.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gensczfeg.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmxikbl.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gggkyxgpt.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbepfliu.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gemvwlsut.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gmwrpcmlt.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvozcwwca.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxzvuuud.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrtwvejr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaxaeivm.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggqaoyphe.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbynbwfte.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/grlqkipow.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/giwwqgbst.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/grjvvimnf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpdrqpbs.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gctsnztop.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqfwtskf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfeywvhf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gnegwrnru.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilrceatr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsegzofby.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gvimlogue.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gatantzns.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gwkkfeqla.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbarxjrk.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdqdjghlj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnamndtri.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gughcivxq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gadwjjokb.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/grzszatic.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gokniqziv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gflebamux.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/glromjmkh.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvthqsqc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwncvky.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gkddovfaj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggeypitod.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyyjrqbv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntkhszh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gclnkmxtx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghztjbfhf.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gahqwkqke.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxchywcyw.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gjgoyqvvo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzhibrgx.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmjrkgqg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gocusnjfp.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gamwkjlrk.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gfhjubasn.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gytouywbh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhexoikd.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/glcpgsqyu.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoybupam.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkogrfllt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/girtwxcgo.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gawcgezvu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzknzaro.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/grbduwiji.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkexxcjc.sHtML


<!-- 参考信息 -->