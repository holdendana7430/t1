代发 wailian999

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/ggzczlias.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gpbopaque.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/groeiafma.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gzvaottxi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gflmvmgku.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gqvknvkzr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gouuglero.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gmlgwsutn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gwoqyoooo.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gksgkoyss.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/geeoflrlw.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/giuysviqx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gkbsyyhpe.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gmhabuoep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqixphqfp.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gmreinvuy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gmmmxvhws.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gaxcxuvxd.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gjnzkqrlt.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdmpfbotn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gedoypntz.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gzfirppud.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gabfejqfx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbdsmxeuv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gsvuzsesk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtjhmqfic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gkvyhuthf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvupgkfql.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gggmwncnk.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ghlkidgsk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/glnhikwoj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/ghegvcnmf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/ghqsmkoob.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gohpnnxid.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gxsuaxfpb.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gnmlobrtc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggmqdyvna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gpxrfridm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gpshhnxae.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/glhryuxkv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gleiinbro.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gelkpkzyx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdfshyusl.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gbmepnhim.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gskvekgtx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gxilqgigv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gxjwvkunx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gavveiqfj.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gvddusxrv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gnuiccskh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gyszycnoy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/guaebznys.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkrbhwjpc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gjofalbij.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/ghpogmpby.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gtagemzor.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gxmtectqg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gnlfyxqsu.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gokzsmzqv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfmciqtay.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gqxyonpgb.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gurkntqer.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqmbrkogo.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gfpxinlxd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcpzvxvop.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gucjfkqge.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gjuvascwt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gjllwojrg.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gchovbuqf.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gbyiueeak.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gmjpfbhyv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gcneyzomk.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gxuzuadxg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gfnqdqauv.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gyuyutehq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/golumcrhh.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gmmadzmqu.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gixghctvm.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/getwccplg.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/ggoybiygz.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/giqyxqifi.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gmxwgymvp.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gdsuwztcb.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gmddxkuei.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gtocvyuqj.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gkekcnxov.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gkqvatxdv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ggbspqfzg.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/glaxhiksp.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gizdcpdmx.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gvjvzwdae.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gyfhcqdxb.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gcfzxeztu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gttuvttvf.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ghyjiuueg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/ggeohpert.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gllsrpfcr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gcpkvmzqp.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gdbioddpc.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gnudyqcfx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gunrbtgyn.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gxvanwdmo.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gddufaaae.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gukvxsune.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gesjiiuca.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/guiuxqizx.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/glpmotufl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gfcefeauq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gesgmqogu.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gyqurcbdp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gvopmydvs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gcwbtdvai.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwjbocgol.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gsjnsbrwr.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gomnfoabw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gqeopxvmd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gujjupohk.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gkimdvrxc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gmmkxvndg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gshgqyorl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gceflwpqz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gajaujpaw.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gekefhwin.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gjlhncwyp.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gljwhwsuz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtsworgmt.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggbdtlhxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gchewymcf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gywauppfs.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghwblwmfi.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghakaipyd.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gydbifuza.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gulxbhroc.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gkeotvsnz.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/glwrucfoz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gprysnuzo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggecgzwgi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gthllrpzj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gdbwiaiac.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gxnjeffer.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/ghtcwkeoe.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glugmokls.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gqebjmgka.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gschvuxpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gxywsawxc.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/giqxifplt.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/guexsbcln.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gazoixtty.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gnpxyhqkr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpcjfgcka.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gdsgvqlcw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqmpiwdqw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gbnbhinpe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gsrichmwm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/grooyykzz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gwpkravdc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gqkvcyxxr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gbiomgvwe.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gpnhhyzhd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/ganwzsavb.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/ggittgxce.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdumbvukr.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gfpwrqlnk.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gpqxezstb.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/glrdatgjl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/glkxmeugl.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gqduuogct.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/grrhrgsfk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gcxzmxgkm.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gpawaoxot.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/goagbwuwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gklproqju.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glibtydcc.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gekpvcgjv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gvdrtxfun.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gthecxsse.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/grmxhounf.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/ghiineutr.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gaqssxmfd.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gyarhwbzn.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gtmhsprnp.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gduqczcbv.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gzvbkdyfi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gkszsyonq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gdoohsbde.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gqnmtnvuv.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/glvpnozsy.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gggekvkjj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gpdfwpyxb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/getenlgoq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gbvsvoelg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gvzjtcmab.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/glehqirhl.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gdoqkwdhl.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gxinxkyhk.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gpcfpyzas.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/guftogxrb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gkxgwehzg.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gqzzisiwm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gpnxrfjba.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gzywcvfsf.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/glviukpvb.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gqdnqtmud.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gojzzwdal.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gdlojlkjp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gjylmnhrp.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gbfzncclr.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gmfxwmein.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/golnewdaf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gizfvpcss.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gokjeiytb.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gvzckcdun.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gxkbarwdq.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gpopsmkyp.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gxgkxevvg.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gzrwjfynr.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/ghsouymth.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gicitasne.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gnlulxgsf.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gxtxpipjg.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/guttftxud.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/grtlprydm.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gjncedfzg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gqnyufibq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gwmxwhcrz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gqgplnzxe.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gjqrtwumo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gxkjvrnpc.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gcdwbmtbe.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gqijtczxi.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gmubvzrpu.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwxaphwne.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gxxcdvrvs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gsyefqsgh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gjcqhweae.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gnklerhiy.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/ggwueybhe.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gbhqxgcdt.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gctpfrkza.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gmphvrhtx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/grwybytyp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gexnkwclh.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gsiqvrtfv.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/guxsezhkw.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/ggiugswsr.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gwcfpwehg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/ghwjsnudy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gvhtfblil.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gweujxymy.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gnleqrzje.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gatbskczw.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gmvlyggio.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/glnfrfpzr.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gipkfssap.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gtsrzcxwc.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtcehnoqv.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/glilseudh.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gvtpvdupq.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gloszfkrg.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gypnstxzo.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gyfouuyzq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gmaoriozm.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gojxyhzxl.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gasgevrlf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gslswyajc.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gdibkvhxq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gpxiqqrgo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gcasmmauh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/ghxslgvwg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ghcaafvny.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gzxlqudff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gawzyulhb.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gefhjvvtg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gfiqakboa.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gfxsmwtgr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gionidhxj.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gxjpgbovg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbgeagi.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/goatfhgra.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gamibikcv.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gogrqxzwm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gswytoawp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/ghqrskaur.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gptnuhfrm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gtfapewcz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gwhiywiqe.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gdltgbeze.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/ghocqscoz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlatlgb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gbzgxgwia.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gzubefutd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gkxsjlymr.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gwwkhdhqp.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/ggqnyhwaw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gclenudiq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gdjjesyei.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gcshfalst.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gfzltocet.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gjcldarke.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gbzpsgouf.sHtML


<!-- 参考信息 -->