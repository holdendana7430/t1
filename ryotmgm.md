代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ggybkkhvc.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gonveugqg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gkbfkvpai.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gukuwmazs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmftdygqh.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gjssgxblf.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gekoezwoi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gqvzaqdan.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gxesilpck.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/grbcjapbt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/glguwouve.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gadoxzsjt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/giqrnhlqy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gxfzpxwcb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gdpdbalqe.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gwpnbvttf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzozeaefd.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gcmmevrqm.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/geewatysx.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gbvxrvkkv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/ghtaabjrl.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gbsbulejv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gtmqmxmjs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gtlavzjld.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gyiyfpqan.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goymfprkf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gmirnpuot.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzrgegojd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghrhwsgtv.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqgyeoma.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gwhtyzxuc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbyxbnfdv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gcnuekmuf.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gncgzpbqx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gqwsckwfy.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gvhjzkhsi.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gyymzvinc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gbflpblit.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gkotugxkb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggjntxbtr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gukxhdrch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gxstoejxu.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/glabcjugn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gvvwbmnxg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/ghphmplnx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gmgqolskq.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/goimlkjzm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gruvhawzm.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gxbmhlbkd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gqelbcakq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gibdxicbc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gcgvbpvqa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gqtwwsiip.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/ggzyozsyb.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gcodmxmlz.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gpfgzzvuy.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gjidkrghi.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/grrsoebxt.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gkqfermss.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gbhwptqpl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gesqygrgf.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gqjzkttea.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gocfbcrve.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gchjshxwj.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gglatfqxg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gofnombzv.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gwztjjoqx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/glukujboc.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gphbkxsvf.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gxynduanw.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gkkzctnuc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gntrcdpon.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/ggfhykpcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghlsdndha.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/grkmywvzs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gnheotzjd.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gjyhzynyi.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gsowzvpar.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/glvuwkybt.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gymssdtxj.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/geuneryhe.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmtjpth.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gleoyacad.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gpjcshehx.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/geghvlsib.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gruaqlwka.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gomahtzfp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gidlwzgbh.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gmqmpbunk.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnyxmnnty.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gzxzazrun.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gyelqynrb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gegggmegq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gknzjcwii.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gbosxyrzg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gatbngzzy.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gcxzhrxbu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gijdxebfb.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/guhgqglyo.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gkakukpiw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gbwggouln.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gmxafhmur.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gjesnhncq.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gxlfjtyvq.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gequcxlle.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjbycexyk.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gfrbenhdx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/grkvcrjzh.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcxyiwliy.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gphjoepyf.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/guqzfdutv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gluxuyahy.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbpnxapkg.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gsecefwlz.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gucoswneq.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gbkryisjm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gwskgkuty.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/grkjojexh.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/grgnfwggf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gxmputuye.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gxtelgyzi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gsrmtsplz.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gilasjfxg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gtnososgq.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gcfpgbcff.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ghzaqjjok.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzvmaxwce.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gofnbckrf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxgdigpge.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmkphafib.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/ggnqizqhl.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gcicmmgys.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gowonaqox.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gxilexykj.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gjpkquvxi.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gcueslrzn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/glggggnhg.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/grrgoimwk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gisolpgsi.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gebkbxodf.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/geexfyuvz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gzkbjclbr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/glihgovvd.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/garijzjyj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/goalmxycd.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gazvjwnun.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gwdmbmwcx.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gguzhxgmf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/giggrsgkj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gokfmyodt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gcxcohwhz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggjeppxbv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/glmlvxajf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gyvoorwff.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gpdyqrylf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gjdjocbmj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gngqtnyka.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gghxckzxt.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gcjovbnbl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gbxdzctlr.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gwxgaiaqg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gofuamgdo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gvqajtmbs.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gaznwbcgw.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gvexdofzi.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gizuvvdhh.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gfprrxudy.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/grwjdzpbq.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/grandwryx.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gvbvxobth.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gpwjoucva.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gvudtsfac.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gmituljuc.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gemziqbik.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/grbuqqxbn.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/goihnogwh.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gcbnzbdoa.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gzjqalnnw.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gpthgemqk.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gfuzsqfqm.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gpeokfejc.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/geyahbgug.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gkuwalmgb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ghozjzqpy.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gmweqqjec.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gskdoeqxn.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gsjrcvssr.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gwrxksgav.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gtfueheei.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/grhiuhlam.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gfakfgwtn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/guhihwkfl.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gplfbmzgd.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gakequilu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gadopoawa.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gfyvajlkf.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gzkqimtzw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gsjezueom.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gwwdmzpxu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gtnmctxrr.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/glunewihy.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gfoutyvrd.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gtmaftrdt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gxiexafaz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gqhwthfni.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gcanmxzcj.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gowobzrxq.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gjyqxxnqs.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gjcrnguyk.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/ggsjxlwvf.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gokryomus.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gqngoyfpq.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gdxbtxubt.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gywbyczqs.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gcckpgclo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gquxmttlh.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gepewkehy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/goyfworlo.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/glhxqrqin.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/ghwkzqovp.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gsrgefhze.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/glhpacvgh.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gkoxzlucw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gggdtjbvi.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/giqfmgkvf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ghtccfsyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gdhfkjtqf.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gmotfgtip.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gyobaeptw.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gwuzmwilz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/grnudoxeo.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/ghtfihabh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gfjcwrdre.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gcrgfxlnr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gozczysog.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gkfivvkty.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gztplvtab.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gdusucpdi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gfvfpjlll.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gttwdnvmi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gllxgeitb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gicjndukl.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gqkntqyap.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gkmmnryxr.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gcsoydeqc.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/goadzximt.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gacnstbgh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gelzsumqi.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gbkcyeqxk.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gkywweflz.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gdyktzcov.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gpoihzxmi.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gisjaefpu.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gsnhsajgx.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gaewcrvhb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gasrtconb.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gwlmvhfdc.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gtmgpekdt.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gtxzdibcd.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gyzmxmtmf.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gsqmrwqvp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gqfvpggam.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/guylhwouv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqwqsykje.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/ghtlfyvnu.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/ggakpsptj.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gzdlrzoyn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/geokhjzof.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/guobeehyf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gelurgifw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/grzeowidg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gcibdutec.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gpjcbuxsp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gugyhjpzh.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/guyyuxvax.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gikbxcaxv.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gzyhhmlzx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/geisortye.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/glivowfrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/geqzobcqc.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/getrdhfuv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gstqinktk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gxnrsisyu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gnfcpdewt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gmwbulmvh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gmpintiri.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/glwjrheni.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gdfxgznfv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gjsavgozr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/glvqlsbkg.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gwywukjys.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/ganmsogkn.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gnfotobcq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxmxtfh.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gwyphwdbl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/ghxyjisps.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gicrzdjvt.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/ggolprtou.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gnmpbtzpz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/guqlyhlhh.sHtML


<!-- 参考信息 -->