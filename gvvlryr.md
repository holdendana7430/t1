代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmmpllfa.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gobhoxbgu.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohrmukdl.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqqwmvgh.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjukfytvp.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gewoheodu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevmrwch.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoeojlzb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glhqyllxr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmdjjggpi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/glqgxstod.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grfbwnjau.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkxaibjjd.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggfpake.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goezzaskj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gxfhwxtsu.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwqhmjyr.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvcqqzth.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxckrureq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxzbwtxu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/ginddwjzn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxwzpmyg.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gausdcscs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gonzisfgx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gbipkbjcd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggmihhwcp.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gljxvcems.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcdhcfuj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzcolavjb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/ghwolzrku.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhdmkuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gormygbdr.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlukieil.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gxgcscaep.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnonalz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnjtcsyd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqylsyn.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqasfayk.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuskbmcn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvbtwewh.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gaplhtwtg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhjnurij.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grdckxkmx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbbjuhhn.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gmuugtfcp.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqholup.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwrbjbfrg.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gvmosbpte.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gfmmixqhh.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkcafupdt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcokwxx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gplarletl.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gylpethhg.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnswxkcrx.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdznmjrgt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxwboeno.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gflqstalj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtxwvlwy.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/galchgsip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/glyrdhpwr.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gcliurrxk.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazxhhprk.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggilsgtqv.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/goewiqhmd.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gdivcbmhq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmzgwedx.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrattvxl.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gywfhhlvn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gfayivzxl.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeuotoer.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/guwzaledc.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjakuybg.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grbxdqulx.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdjztiidu.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfygiszvv.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxugyluo.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gzndbfzie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/giqfksnnf.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gzkgujcja.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcifhhbi.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjwnqafb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttqdcdw.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glajvcvqt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpjymwso.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadzxdati.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gfukasdci.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzksqjmyw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmofltxpo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggydbhfro.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgnochcj.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqtzkbbm.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gezsmnoee.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glzpmdjbc.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsudmvjx.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmsnesor.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhqhcvc.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gbfyamiel.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmvaucah.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/geukgfyih.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goenlzmhg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/giovxjuzw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjiakid.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdduscbki.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqflyaluk.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpznnnhf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gigeqlrdc.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmntkvhru.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhkuhdjr.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/goverxwfp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvhcnmjb.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqvuqpsw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gseokxovt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmliwmdu.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjiqnvsf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbcxbccd.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giwfrgznb.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/goqymtfvf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gohxpswqu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmqcajfls.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiarbejj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwngdbyqe.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/grzdfwsrc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkxruifd.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/geftrirco.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gphfznyza.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwuqtefq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwzqeaate.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiftbxuo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gjvmuzyux.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/grnlaqpqf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvfmwulm.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gbtsfogsw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjnwdums.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwrpeywkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjblhnubh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grsrbcytc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gasfuyknw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gvoafnpbz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fanxiaobao.xyz/Article/details/guxjhzhuk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwnutjsis.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjxjhkk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gkwsvmhcu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/grgxihqfh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezqipuxk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gwxrskiyj.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gychkjyxo.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfycbxpb.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasuxnyea.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gertnkpli.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkfiqzc.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gpfjixgdl.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcvbqkrg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/giyuoxgbx.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpsgiuuu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmylcgxwc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gownhlyjx.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdrestod.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoxejryc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjxsmksi.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsveejfs.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gburnnhyx.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvgpmnty.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/goiqdgxzx.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goorhnrlh.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxffmwh.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfomcmzhw.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gxyecbrlt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gentcotgy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmzpmjh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvabxazal.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gcyuprmua.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsrmnull.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gordkvqri.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqrijfhv.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhwyaizr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwnyvnvv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gsocgncfo.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gkmrcofyt.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxriccud.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueiucnta.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfonlvdtk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/glowgmrxc.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gusbvwtgd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrubyuem.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gujsqwsbx.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbxuwyxx.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhwptydg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gyegirswy.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwicghczi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gihoxglwf.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gevrliwlk.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ghidgcyjr.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/ggtmdwvhm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnmimgzb.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymurweia.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvtbydyd.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gjkxpgvpf.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gvlubyroy.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvlfkgwo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gzloghhmv.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gttgbwavs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkbgwidz.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gynenqyzh.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggynxqoxz.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gtlkmepot.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/goydfktva.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkseqtppx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowkxypgr.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gatrbplon.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gagjjrobo.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gaqowcaff.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gwgsyhovg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gacvmkidk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwljzovo.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpjzwhyq.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/grgqrvrvl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscznktue.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gydugsevb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcivicpv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fanxiaobao.xyz/Article/details/ggfvjwhfl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmdrcywn.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gocxrvfwl.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqxzjgtm.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gydqwucnk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/ginizztue.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhpmourb.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwvjtmcy.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gphxnrlqq.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhmiyubd.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gqccfzqbr.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gnynnpgps.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqxzrpdc.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzgpalqh.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/grvntbkrz.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkrndfg.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/geqbtjfgs.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbiuiwmo.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiexhoya.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjryakjcr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqbusqmv.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvemuyrr.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gliksrhwb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gblyfxbpr.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gleieudkn.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgtzgph.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcozpmcrl.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/glkexyzhc.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfctpdws.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdtbpoezx.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/grpdmxvwk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gexhgkper.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpwjdhsk.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glstqsolz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/grxjzzsyn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gdifkvbff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghotcydzo.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gbzbrrfdb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gublojrqc.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gnggpgocf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggpiyxvt.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/griawwwaa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsltxhdy.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/goghhippt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmsfpnuk.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrwbxwmx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guejyntoq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gxcynlvuu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeydtxbz.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gljzzqsfd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblkytmrc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnbkrogg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqqjzyee.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxgiskze.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gomjvyuuk.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqtqbplr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gnyptkztx.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gfjbnygdl.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gtlzfeeyx.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/glatgfdma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gogkvtiqt.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfucgysep.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gjphuotni.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqawrhcaz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gpngpvinj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govenzpgg.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohldzos.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gagwczugp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/galmpakpa.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gcffxboqq.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gzovwghxr.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/geypnjtwc.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuyinlot.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gkloojdjt.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gkkrdowdj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gkrrwcjsl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/grduhfucj.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/golilwlzf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtchwzgmd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gszjmpirs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gljftajht.sHtML


<!-- 参考信息 -->