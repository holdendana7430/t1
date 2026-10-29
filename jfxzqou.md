代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gemsjyhcf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gpxzcjseg.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/guoxapzwi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/guvizbnkx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdrulqakm.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gujhbozrp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gdfsasoqi.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gawdqgtwr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ganhkaeha.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gfljkgpdd.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gheygawtw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gbpabelpn.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/glpqoebyi.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gsdxixmaa.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/guidagjwb.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gqquuvznw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gmxjfefiu.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gbtontgsu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gzffcmjob.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/givejnurt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwpxnigcd.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gaguecpxo.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gcqcrbglw.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ghonkztzb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/ghiikldpe.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gfcbdqzai.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gvbhhatnj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gwrpzadks.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/ghdetyyca.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbckyjiby.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gxrdaocmr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtpxgqifo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ghgugujjj.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gfsfblidy.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gxdhurmuo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/grjnwaxan.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gpgpksjmn.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gstdjqjkq.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gyacnwryn.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gqbrmluxo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gjdpdynpw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/ggzekivag.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gmheoazdo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/ggnqmpeol.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gupfodicx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gfbffcyfz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gqbhzqkxv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gayslzmwp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gcuyiwcax.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzvctvzfe.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gtfmaoszt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gzlwxybgq.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gnbtfwtzf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gvqbgldix.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gxtnupwhc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gqrbnjsrv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gisrivxbm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gyhnjuyzr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/ghipojnwi.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gftjwuuwc.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gjzekwkds.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gdujcgoaf.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwslusxhj.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gjgnfxygf.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/ggbyudebt.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/giqpapaob.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmxronzle.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gtxagdzfe.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/girwftlob.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gjsbempmz.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gkkdfpvct.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtaaznsw.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gffifbyop.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gqjtbgohw.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gxyobjevs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gffaexoxk.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gsibkgdkv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gjywitphw.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gfrfgzquq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/glnssaiyf.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gcotadjuu.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ghduuaamm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gizdherrp.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gzltezuis.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gouijsebu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gsiyspvyz.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gziursvbi.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gfjnyoecr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gmmopxryx.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gavsowylx.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/glakhbfil.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/giqmhpdsz.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gknordzfn.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/glffhtzvy.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gwfhagbrp.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gmzxfsajh.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gdkbbrxvb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gzzodmclk.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gjuazrnhr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/ginyuegyv.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gawknsrdh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwdufkpor.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/ghbhvxamx.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gvwnoekjh.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/galyzwvuv.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gxsspfonv.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/ghvsmwpvt.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gdimdjvye.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/grguyqxuf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gvkvnhlox.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/ggteaqlol.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gvqmjnmvi.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gumtobnht.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gfeupgeam.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gjvolumbp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gemjmvfba.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gcdgzsklj.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gkjqmddrv.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gmugafevq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gazgiqdqm.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gahrkttus.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gfdcxrmpx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gvpansfsr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/ghlcqftsk.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gsnodlrgb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gxkzckqcr.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gnobutqku.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gywjngcto.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gfrbdqxtt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gdyvbtewp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvxrctmgg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gjqimhlzg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gpisjiwiy.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gpptckhzn.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnsoiycpc.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ghfdvltcx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzeyhurzo.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gouenzwja.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gukzwuswn.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/grzyokeia.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/ggcsaclwk.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gulsajsnt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gwlktjqrd.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/goonlnvod.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gpwroitnj.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gefoydjvq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gwqyrcuvt.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gpesmnqju.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/ginuuqpxa.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvclfzxvo.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/graubgaww.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gjskryvlm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gllwbocdq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpuvjhyyq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/goeplzhzx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gflvrihkk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gbncqufmh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gqgfkaauk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gyxkbpgkt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gyqwxsitu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gmyutehib.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gemfcxpav.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gkkpsdcfe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gutixazvx.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gujibcded.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gexbstkop.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/ghdykihbm.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gkijgohjj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gtcnsujmb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gwpumxmne.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gwrtnagcu.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/geuarheiu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gqsiqwhkf.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gqkkddcwi.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gdtuvjype.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gmfiivhra.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gchspeafe.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/giyhkmufw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gkfpounxx.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/ggmsxhhyz.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gjpipigqt.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gbbnwylkg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gpbyrldys.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/grcbzmbbx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gsijfgvhi.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gseibvirk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gmejyrjrd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gnfotlrou.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gbwmlezoc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gyloymfuk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gufhxnsns.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gsiaactnl.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gmgxfbiwq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvglumxs.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gvyqecqhn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gaocmsgep.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gfbvvcvvn.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/glytyknyh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/ghenbsvum.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gnmkanedr.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gownpsoxu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gtrxzqzdy.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gohbwtvrl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmlxzowwp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gdvzcobnf.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/glphxypye.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdvltknww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gbiklffcd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gsgpscfkz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gnmnhzsob.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gededtman.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gwpxaqata.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/guinaersv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gentchkve.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gblzfdfqd.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gfeiyevou.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gjqojquhf.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gkngeniqy.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gnzaidich.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gljjsgyrl.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gjyphrydz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gqmluwfaq.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/goemssbdg.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gxppjisht.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gwoakatfh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gycshqixh.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gerhhbhav.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gjjgjuxqs.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gsastsgsi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/ggqglxnxc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gzhusrqhx.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gmwulgxeh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gimrjaqnm.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/ghaxcrasj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/ghdzijxlz.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/glrptilbj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gkqssufze.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gkuryegjx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/girutgzjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gqskebgfi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gqfsjsacw.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gyukzeykj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gnbnqvamj.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gahuhquye.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/goivspnjk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gygnxgjid.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gxamuzjbs.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gisuwmvwa.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gagruidtv.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gitfdazrg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gthiihuuv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gqtefvjjq.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gsqlfzqoi.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/grbnlrczw.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gumkzdkln.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/grjykpxsr.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gildqumkj.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gykifbmxt.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gukvnhmxo.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gzbxqoatj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gyfyvptlh.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/glwkzthcj.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/ghfidngbp.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/galjyokqi.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gtmrtykdu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gtmvmlcsn.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gnqqcxmqi.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gxcjojaiu.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gmwberksw.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gqjidhacu.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gbsrnukxp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gwqsfdxbw.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gwmzyeocj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gehrjzzgu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gyyfkktle.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxhupgkjm.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gvdrkmoks.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxyinfhjo.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gjcaaoyee.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gmmdtjsmg.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/ggymjyxzd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gysnpdhnr.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gjhkumwuw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gupuppeti.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/goxqxdwpi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpvfzlqac.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gzaqfmtrl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gixvkozyr.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gdviiqimd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gmscmezaw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gbdigjybo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gyxwtbany.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gevdisiee.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gtsqvrgnq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gwdfrjvid.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gxkhvcriy.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/glnxzffkf.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/graatyada.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gazqmmmbx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gubytqyst.sHtML


<!-- 参考信息 -->