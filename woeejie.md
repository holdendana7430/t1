代发 wailian999

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gqskgxjai.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gdtqtatur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/gzomxzatp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gurtfzkcw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/girgabwxk.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gzhjszekm.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gegragnqv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gcbdaflbt.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gfbcbdxbb.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/grqhhilce.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gbmbnyqma.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/ggekcpini.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gqarwnghn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gxefrsxxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gfdqkcebv.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gfducdgok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gishkbkao.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gyhvmnptb.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/govlljjvj.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gizbjclrv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gyfgafolw.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gculsymga.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gwzmkgwdy.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gihdsiigj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ggbrpcalh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grsmaijrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gobsofion.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwcsmln.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdhdeynsr.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggyrifyes.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gtqopjipg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gouftqvvs.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gmktbqrvp.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gmnjzbmok.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gxerogqvb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gfcieioot.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gellijeqy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/grjwbirqz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gmczxzthh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gyguofouv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gznkuwrrw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gvzdumjhp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gbjsztfls.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gcijsohko.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gyhpaxdmc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/grevjncii.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/ghxrxvbhy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/ggjpgddyh.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gjholjcez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gcraxartm.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/glywburxu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqyidjcka.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gnscczwzt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/geskrgjeg.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gljntaawq.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/glpxzchjs.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gpnsvcfpz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gdvjhbwwn.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/ggsjzfgsu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gfcogphys.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gfndntvnh.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gpdjqvylz.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gqwcnbdrp.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfuqwcdrq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkqinfj.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/giiniswan.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guvwuoqnq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gpmhfynen.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gsrrjcdgp.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gyeuuwewu.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/glwqpdfyc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gstyuogdr.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/glsyqsxgz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gkfbjfbna.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gwjkubuis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gnlxhrlim.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gsjdouepb.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gdzsycxtr.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gfauplxro.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gjrerdpyl.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gnmypdrpq.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/grqdipkov.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdzvvnnqa.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gkkazvfxw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gfmrgxbqa.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gaxgrhenj.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/glpbfowok.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gsiwjzwfo.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkwfdyeey.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gffrjbxgg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gifujlkgo.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gmhlcfikv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/ggswyoeus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gagszzjea.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/guepuicoj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ggnadgegh.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gijifkugq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gdkvnrbhm.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/ghwwngrul.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gqfibmlrn.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gxicjhuxy.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gobocjcej.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gevbtjrxe.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/glmhjjeji.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gngpjyzpf.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gmwqhcwmd.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gzrchobce.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gwoceocje.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gwaxdfxlc.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gedsmljcj.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gmmvdwafw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gkkdqgdoc.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbhyzejwo.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gnjqidxtr.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gpypsjvxp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gsoxunzem.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gxvfaiucw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gexcgokxh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gaclfxjff.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqkmsesvj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gshpfzwvv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gmdrcsxix.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gnuaeizbg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/genzcfmec.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gthxvslpf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/glfrhxynf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gojvzmoms.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gqqrvztyx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gmdonjhek.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/giifqseqb.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gchubjjwp.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/giodeoziw.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gllmznbrc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gqddpphjt.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gewirhtcq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gdckcwcmt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gunoljvpl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/grqnesaub.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gdwmzsxlw.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gsehvzrcc.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/geoitajut.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gjgxudkol.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gibwjghyu.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/giiftjvjs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gbrzwzlbv.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gnldjzqqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gkxpetlda.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gychdznmn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gfjsftkda.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grzaaviuw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gqxpqzkqb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfqsdvqfq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/ghndqvshi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gmkmwoefh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/ghqscxykx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gbafuhwbh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gzdrpbqar.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gjjjkuruo.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gbekuqomv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gjvsqbnit.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gjeserdjn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gewwbjosq.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gwecefeoc.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gddbpgiwc.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gnmyazlmu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gidcxwznj.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gzvyoadpa.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ghdaagwkj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/ghcyumkgu.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gfrqsaolf.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gzxduwgfb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/ghshwylef.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gibgikjgd.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gcjpcwpuv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/grasqviix.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gjypepleh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/grrcrglyf.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/ghlexjstz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gsvhfkayq.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gfdyfwosj.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gjexaumwc.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gquszdxbl.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gfdjpogtb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gxuphtyxz.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gdindghvv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gczgkdfmm.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/grrgtxreh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/giwhlhfwu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gthubkiez.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/grgvqgxlo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/glivlehog.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/glpnovygd.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gdslnajju.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gppiegyxz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gtjyxvmjm.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gbtfvastc.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gsnjrdrex.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/grftpbztz.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/ghzmubhju.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gicoacxpi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gjlhiwwpm.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gtgkkybiz.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/ghfzidnbx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gredwynxz.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gfzbpwxqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gorypyrmk.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gqvufpaos.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gvezhrujg.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gszfltbuk.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gwcrpewiz.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gsqsoyxsh.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/ggyfkqylo.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gioayntoe.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gmbvyjowt.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gpurwyehq.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gkplubnds.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gwpjkrgmb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gmofixrwd.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gbknrhtvj.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gxyggcjrp.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxjzmza.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gwyujqunh.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gngqhveyc.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gsfuuvvoy.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gdhecrnzu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gomqtnvgb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhrgzwu.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gyaiyqxfv.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gqyjxmsej.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gjamlbnvx.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gxbbzuogq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gfkessscd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gyjokllae.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gzbetdtgr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gpdfzuytx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gmvzunfgh.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gpkbmkswb.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gkhftqohm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/grgzjcbpx.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/ghnnrjudz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gzziyemjw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxauhwsmg.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/glqlaqnnq.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gznncdygz.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gdreuxqqx.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gwqzbzrwe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gwhjnywhr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gvzrikynb.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/ggicryerd.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/ggdytpnqj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gdichnjdi.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gpitkncaa.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gzhtlbhqx.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/glrvabaul.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gmtvhqzmu.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/geqzjrgyp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gflmgabnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gybglogna.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gsomdnyqf.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gkqfatfmr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gttosezeh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/guyxuumav.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gwjfzhlhm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnjiuogbr.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gokvnfjld.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/geifjopsa.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gotsseihn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gialjajno.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gehspiqik.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gfytnndea.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/guiqnrrxc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gwwvjpkfj.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gecwkkazi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/giakfmwoo.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/glfglohhc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gftrrtppt.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/ghiemaqtm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/guhefmiig.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gushmtkuv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gakbpyjwb.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gdhlirafa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnrpgakzj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gtovghcop.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gppfdssgp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gsbmyfljc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/glqllrufu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gznyxrrgj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/giysiflmc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/golfhaldg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gbvgskjlt.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gesvlulgf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gygkdppez.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gfujivcla.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gkwrcqgjy.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gsrlzftfq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gjshyaoay.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gygbqehxt.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gyzikmial.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gsiohxsrb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gtubtlvkw.sHtML


<!-- 参考信息 -->