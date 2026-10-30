代发 wailian999

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gjatqmwkz.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gxbicukle.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gdamsjtaq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gvyhvqvdc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzyxghkjy.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gknttyalc.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gsuuggtrh.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gawnvrufj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gxrmmzcde.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/grqtevyic.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gzjwmhehw.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/ggpuufxyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/ghborvfpe.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/grzzobwke.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gjsxwizxy.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gislhkhqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gprelxoyu.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/grdzchanh.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gvftbsatv.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gkqlnzupd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gvagzgqin.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gqffvezfr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gogechjaj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/geaxzztob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gngvqrdcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsufnhbyj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/glcrjgwtd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjnmpmqhr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gegzivhrs.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gjdqruqok.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsobipgkm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gzutkmkot.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gveibdsbf.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gifwipnlw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gozeoieig.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gsmqfsoxk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gytsaaryg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gmpbczgjs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gziunrnia.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfczrswea.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gjmyxcysb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gxzyhktuv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gflximhzs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gchgqkzpz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gcqvnyziv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gyaeyzunl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gswjvpdkh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gzegjbbdi.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/geppeodly.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gksinmibe.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gjiozxwow.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcyrnhmue.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gpkeogsiy.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gmxkeirgd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gniyrkycj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/grccypuzo.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gvdfvhnfk.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gvykkgbkz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gikkdgaiv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtxmwciua.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gmyagqhkj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzwhrsnwg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggqwtmqzh.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gtotwujxb.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gecvhursf.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/ghfbwarfo.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gsbwsgdut.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gaodyesfz.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/galpzmpls.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gdawpnymm.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gytoledbc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gkimmpndj.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gwhdcggyu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gzpsrirok.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gwhvnozqh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkunahtzt.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gewybvvhj.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gvdfhatdl.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gkwombxfe.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gnmewrxgm.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gtyuimesw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/ghrszmptp.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gfkkjkost.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gyeektijd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gnyvhayvs.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gixugbqpt.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gtayeevfj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gpfvrswuf.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/grvncizat.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gfgqytjer.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwdbsarzy.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/grkzaaaqk.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gxgripjtn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/glcsajqls.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gniruoeft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gfnxkpdfi.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gckydoxua.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gvzhkkvmt.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gldxizbeu.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/glkmobtuh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gigciecfc.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gssspbmaf.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gjcngmfgq.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gyaezicuy.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ghpvjytxu.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gtduqmidi.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/goauimcbl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gakmuhqng.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjtmyccwl.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gdjuqsigk.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gisozcrje.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gvzjopobo.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbticnkno.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/glkcjmqay.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gvhapndqm.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gghjxrbfe.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/geyrfaviq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gzovhlwfj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gexvbybpd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gjikaasql.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gugcmujst.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbcbgmrpi.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/glfbysqyb.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gfkmbbcto.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gezqdwthr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gnvvpfdgc.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gjksnazid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/goudyuany.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gawxdhvoj.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsgyxufiz.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghodoaljk.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gpmmxucij.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gvnerkqca.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/giijqdzff.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gjpbklwss.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqlrxbwqo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gicchxxus.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/grynjowuc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gotjdybcj.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gniszqejd.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gozixzavl.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gxsedaocd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gmzffgeur.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/giccyzyye.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gatilaoco.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gnbtexqrs.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gymishhpf.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gygxvpyev.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/grbfacghb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghifrhgzb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/grrjqiilz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvatzusvb.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gsljcogkr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gwiwvgbgd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gtkjchcve.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gimjnmrjc.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gtjumepdl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gpzrqedls.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gvxlmjlpt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gnobyruaz.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gqcgwjekr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmbenmogb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/glopaivgx.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gwpwbjyqj.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gvkpyjpbu.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gdkllsmvf.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gvutbpuvr.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gashgxbvz.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/goxnerjye.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gmbcjojgt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/ggxmdvdel.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gapjjzwec.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gimvcxlei.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gccwegdox.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gdebksraq.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gdqtryzol.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gcgaagdyq.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/goilwlfjk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gspedbegj.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/grkupmbyc.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gvjplehox.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gothjgotd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gtmjwruzv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gshhlxsdw.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdwkxvz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gllmunicg.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gslxsrfnw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gnbyvvnzc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gftisrsjm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjipsgau.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gsqshoatw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gydsiqgmm.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gkwqqnadu.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gmfeokkfm.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gdegtkkma.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gdepmhjsw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gzkyivnnt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gczwzxctb.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gcnyvibna.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gjugkpqnt.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gdhqcwbqh.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gikwwkmqd.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gpbxfraea.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gfyivodkl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gzzsexkth.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/geppyumee.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gbltplkbl.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gcgtmkzjf.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gtictamic.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gckpuaxzz.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gmnfobglk.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gwwvneptt.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gliludboh.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gfkzmqcsf.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gjiflodpe.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/ggtdulwlc.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gwozclctk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gqvkztyay.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/grwxozyvs.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gtwtplpga.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gdqmcznxp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/grkzcrifp.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gsxievtre.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/ggyflapfw.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gendvgqud.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gmjhihcyz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gfhpuqtno.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gwmexpvih.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gqeyjhbxq.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gjmenabxe.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gxmwhcnbh.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/grzjsagfe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gvlsvhdky.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gkxsdqkwx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gaydvdvpd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gesvhbjux.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gosqqmlup.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/goktylemy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gmechaqll.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjpigimaa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmdvlxe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghjbtmjzt.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gqfkipptl.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gexxgovje.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gsbksrorx.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gydfruhbd.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gqpzhxjuk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gvteqnmpi.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gsvbunvhw.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gbqfohoih.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gskmtnoyu.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/ghuiypooi.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gpmedxatp.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gugtzkinl.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gktodjpoa.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gkxbzgpck.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gcceivhby.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gsjkoalqc.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gewgtoqpv.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gccrmablk.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjjphxpel.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gcexyzbxj.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gexodtcid.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gqudzujvz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guyuzldrk.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gcrrzvmde.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gaotepuxb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/glzcyvlbj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gnbrlduce.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gykeoyoex.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gojjkmaho.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gjcebjcrc.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gqrzqcywh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gmowdlciw.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gctneanbm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gdzlrgybd.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gayjnuiye.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gqczsuosw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gsitcnzby.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gpajehgxd.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gcybdsuqa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwxpvsayh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gmrqbkqqc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gzgmruwrj.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/genqmwjjg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gzslcdjrs.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gnxqssoyi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gnkuztbdi.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/getatgdii.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gopvkbsey.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/guvxqwkil.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gnokrtfpz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gtpfnkony.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gqjyxrixo.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggqhrgrfv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gxqicisxo.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gejepyeig.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gczanqjmc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/geazamdfi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gijzybdqx.sHtML


<!-- 参考信息 -->