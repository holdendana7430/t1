代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gabqqplyf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkbqckd.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsojiyir.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/glnynisoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gorzhveta.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gxjtxkaye.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpmwjoun.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnuhvraja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gwxpefito.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmyicmf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/glmugrmcu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkumtiqdz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gzafktfcb.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgbsrzij.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gysldauzy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsypweap.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/grmofzrws.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gykzcmgvh.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gselzprym.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcqhaola.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvbgtbbws.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gomphxjjb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyhqtbgq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gllteibdp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gaelqoyre.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmjhpjza.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncegewbp.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/goacenxzb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgnkvscg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihfmdiuk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gclfncqvc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxamxdlov.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gajlixvnu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/greydegmp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaydtvkk.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedzsjitx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkizwnlsa.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwruxqvq.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmtmnylag.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/ginlasdek.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/ghfeiafoc.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjodfzius.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbmofinns.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gisqtvwia.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdibawqeg.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/geyfxsfwf.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdputgeqd.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfwgziu.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gunqsldcd.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkorsfxy.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdsynby.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwhdthk.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxjvgjbh.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvyawqs.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtlvhjvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqphdwob.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvbwmbmox.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzxhtnnd.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwyixvkl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeltwrkp.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/ghibhhikw.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gibcfehxp.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxnatfyt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpblhcpt.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gefxzpcyx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxybyfeij.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmdlnghe.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsqncwqg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gdhztispc.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnjptsd.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gfnvqnavm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkdrxdgp.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdpaebyl.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpkcipxr.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzfgtzmqy.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/ggamyepsr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclcbfjxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gredduccw.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnphiost.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcdcwhoh.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewxeaswm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gserkozdz.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkczczqhq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuyoleap.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/goktfjypw.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebippeld.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxslkuqqb.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gbksfggzr.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grzdffqiu.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsavxiye.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gnhkksfoy.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuteuibd.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiqylwhi.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbujneuzi.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gblrhgldc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeyaaszm.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtadecucb.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gdbmnzrmj.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacxevixo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gflajubbk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwqwwfdr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gthqavmeb.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcpzjwnbe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grhkxleiz.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gdwybluts.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadtroetb.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxpyspxu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcgzwigy.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ggxxorrng.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gijfznarv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhyfiysx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtacvpeqb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlhunttw.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsgyrfeqe.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gqsguleop.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiotbcog.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqnroqwci.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaidelcon.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggleynyzo.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gvwxxgqka.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbmugjmb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/geinpuoqz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyawscvsu.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gzeghiwdq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlmuozub.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcajbcdze.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyycogpd.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcfdkvut.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpmjctcc.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyiudeswy.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/glkhqnffe.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gtbuihfaf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpohbfhuc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjdtxktgc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/goinyyuzi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghrgnysyw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjlzryqtc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gdxqxcwmk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtzatdei.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giskqnsvw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzekkefa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguqhsouw.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/geybweehk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gbmfgabyc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcjmvgbo.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gwijsfovr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkrjrjek.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/geuomwpxu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guankipwx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gjsqfpoum.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiclezih.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfjckrqg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjlduyjs.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjmexkiu.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqgvbpt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozeirsyj.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/guslpowwy.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gppneukxb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynvrgffa.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdwlfhto.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/giluvinwo.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwsknftom.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gulwhayrz.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gcexdhdsu.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpdgkzne.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeydtzdh.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gecqoqxll.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjiqcyey.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnjjuqbb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfkfzrab.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxnmunnr.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gjqddbjjj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gjtbrddxk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/grphnsxfs.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gwshyaiwu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhfptbwf.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/ghqxtirun.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gutocvluj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjlporxe.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgrhsmeq.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqcluwwut.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwsoecrr.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxlaqnjjt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviuujmwq.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/glyqkktlh.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/glridytsq.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gfemaedwz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gzoszuyvf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gkzogsvfp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvfwfapr.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjgdybks.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhnkmbyv.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/govnvfuar.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/grxfpjpfs.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwkneeus.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/grvyejofh.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhqgieoj.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gfjwslfqq.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjdttdzci.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gijfxlbzf.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdtgfzdz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjdcbqpy.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gaazfzzjq.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gdqbwgnyn.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gosnisdfx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gdssjqmmp.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjjxjttue.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuzdstjp.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/ggobxmcnj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gvygfrsij.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gziohwlta.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gezszukqs.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gargqfati.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gckenbciq.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gclovjefg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnqdqxzp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgzlpevs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gzxfqvokv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/glqzmhonx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gonyhtgnc.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorgtoqye.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwchwumu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gtovrjjnf.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gymnfcfoj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcgxsfvud.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggyvxhjmy.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxommlmyo.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbyakbhh.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxlefywnp.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlhpgowf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzymdztp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbxstdzj.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuheeuxy.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzicless.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gpxevmbrt.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqdubcpop.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gluvmozyc.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gcdlxioim.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gipvxobil.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxlyrphv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gebfzexib.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhabxojy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gikxrtird.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gtuznsjos.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmibkvpzx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgltvfly.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gokphmrmy.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gybymatdr.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbgmwlrpt.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyibwatmu.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gpvskrwbw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gkgysxemm.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjtwdkrv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gshybzgjt.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpnpnene.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gfvegmmfr.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gawumurku.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmsteaof.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrpghgzc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujpwbov.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmivtucns.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipuuksfo.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghzhwznag.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gpnmpthkh.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gyckytkzd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhotzhf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtznpbsqz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxxmpejl.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtyhxksr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsortkc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gqomemjer.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gcfmlmtdb.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbyupsm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gosgsziwn.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoyebyeh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfhukonr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvimhqgwi.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gphhinsal.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcpqgtml.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gadoelzac.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtjxpsyb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/golorxzjg.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsigabzy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/giupwcszo.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gpywyliyh.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqrqevlo.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspjxaqtk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gykgyeaso.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gjnhysccb.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gxymqcwnk.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmmrquhy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gbqnsmwns.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadqdugw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwcwufop.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhcghfss.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/guvjmgxwh.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhihuwrd.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gfqxhegng.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gnappjipm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gplyjvssu.sHtML


<!-- 参考信息 -->