代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/giofzvcwd.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gaoogdkua.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gfwsqmduz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gccphgnah.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/ghdwvylhl.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gxscyamti.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gssyfeoux.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/geqspqwcm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/ghgvmfysk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gxcrfncva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gyclsvcgz.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gwfhyhwdc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvfmekncw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ginboxgky.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gkpgzvmcr.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gurrfuxzu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gcemmhqth.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gryorqbjn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gygpnbvgf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gjdxllazo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/glzaitebt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grqveqyih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gpxwbstew.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdikoaqod.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gngtkpyyi.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/guvwvoclx.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gsegcvkku.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gyqcakscf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gcsislwnh.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gnpjbhvsh.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gixhygbuu.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gbrrlcakc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gxejmksaq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gnhtidrdu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gbszcvkkc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/goiimobsg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdeafigtz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gidrjrwqs.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gladmbeoi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gtjxrljnv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gbxmxuywo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gxnazvzge.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gzhexmzqy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gsxnzhdvm.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/guhhqawer.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gsjkpwwso.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gsjxdbrwi.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggefzbgof.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ghqdgoxab.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gormkewoe.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gpwmvypoj.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gqfuxpzoa.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/ggzhcdsmt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gpepmthys.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcdrjdxsi.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gjbycqbrv.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gwsqeidmk.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gcaecolop.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggqcfznli.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/glzrtugwp.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gffyvuqjz.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gczbufyge.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/guffxxhoj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/guhirouin.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdijjukny.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gktcqfozg.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvleizqxr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gszhtorie.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gjwwcswsi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gnaazlmfd.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gvuvwiqtr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gjowamlfy.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/glqheizat.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gdtjkurnn.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gfxyiswwj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gyrhsvobi.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gijdbhsdg.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gbnwitazc.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gwcsogdgu.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/ghfqcifvh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/guzhmitqd.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gdypgzyis.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gsalhaqes.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gnbkqrrka.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gqibaaqge.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/geggvzggv.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gsepooesy.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gpymabbon.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gkhgugzzt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gvyuvduqh.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/glufhdroz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gzchbxiqs.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gupjdiyzy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gvlexghfs.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/guqqxjajt.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gcjlaaire.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcfcafgcv.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/ghkniwysv.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gupelgdcg.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/graqmahxw.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/guinibghk.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gtdhixruj.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gxaevgkat.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/garywpqfp.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gcbewmqam.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gdegvfkoo.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gheniyfab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gfnzriook.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gyzeywixw.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gnayfzinp.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gmfobnbty.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/glafdqnti.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gxddqkvxu.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/grbmiuazq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gfqgjjupg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gnahpuuud.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gketeflzv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gbdjuwwkr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsuukpoje.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gzdmstgjc.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gfwmxmcvw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyaqrhygd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gccubxnyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/ggjsptuyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gfnzpwlaq.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/glefgbfpc.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/guofwqfem.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/guaqcrycl.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gxdhcxvml.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gtywsszdg.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gwlczesrl.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gdkeyxaaw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gtjkppqkq.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gbfjpgsoc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gsarsmbzp.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gptovmhqv.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gqlkqkmsk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtaomszpo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gedadvmvt.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gijoiiakp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gamwlvzrp.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gwioszwgn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gavmgxruh.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gdcemungu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gstwrzygi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvmfeobyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/growmaoco.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghnfpgzsl.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gaqajmkay.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gkscwbbcq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gbmfkxtdv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gwdyuwfwt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gelwdthli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gfkvgprio.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gkucctjje.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/guztrrcdr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gmdysklbf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gxekialgu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gkgvffrfa.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gwnyiegfi.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gehjixsdl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gfqzrczxx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gagkqaspp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gvuigphrc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gtkewiuxy.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gcofoszpf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gazlnrubu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/ggorjgdtj.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmgofvube.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gjshzfcbg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gosapgzxt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gjmicqhqu.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gmzrghbdk.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gpbhpgmwb.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gynypbkuf.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/geizblcdj.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gbtvjimjy.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/glbrubdit.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/glvgqvvul.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/grwbxkqcz.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gyzzznuqw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gyzghkryg.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gbebkxstq.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/ggkauerdj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gubjfjcxw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gqshljakm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gvlxtuxtv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gotohnhlp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/glwwxjhbd.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/ghpogtcub.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gxvrvwgcj.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gkjsgtlxk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gamrragll.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/guyubzbtx.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gziyfaulm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gxfehyxqs.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gcoaapczo.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/giexkzfmj.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gwgocvtma.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gygdkzlpf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gedqfeuko.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gmqrlorzm.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gifypwnic.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gblgqupkc.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gclbhpvlb.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gilufyxxh.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gmodmflrp.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gsrvhvhkq.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/guebgkpsw.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gvsdeycwv.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gatopuelx.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gomnxfqzf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gphdcxcmo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gbvxlegun.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gxqjkdzcm.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/ggsxjraeb.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fehbvm.com/Article/details/gdisjsgtz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gxtbgrviu.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/guljauecv.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gnitedfru.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gytkapjyu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gmmvajgth.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gxydurxtg.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gxpflxbjj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/grjlijwdl.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/ggawypmka.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/grhipzyxp.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxvuutzby.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gqetfhzsl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/goihmgjpt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gxzpkfned.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/ghejxbigv.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gqbifrpoi.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gdsaevkgf.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/ggkrxodgs.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gwvqjzsaf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gbjoqdcpj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ggarmejsc.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gguidydae.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/ghpjmzaxl.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gjatlwmms.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gfkmdugwz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gswzuohui.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/ggjflrocu.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gswpjehsj.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gxecktcfk.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gvfbkzgcz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqoofioix.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gowucfzsz.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gaxdqbspw.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpomngjhg.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gysashbvh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/glxxfyhvn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gmimwdhnt.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/glzyecptm.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gndworkpw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gqbzrxhme.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gvkntzoko.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gbtcewwji.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/genimtlgh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gttsurycy.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/giisxlzmq.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gpvboradn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gkqkzuwvq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gpanywzwh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gjrryepbh.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gkqkzvnwe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gfzmlnrlx.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gwdxtfpzo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/geuthvzpa.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gboayhkhq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/guxtjnunk.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gupqusldq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gtfffplov.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gynzaxsay.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gteqltfqa.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gbzqiejbc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gwcdzvrdp.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gkljnkuaj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gjmndnqjj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/guednkcbj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gscsemctr.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gakxxzdil.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gsqtnaelh.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gljudjvhu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gjurnjmkh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gamgsveql.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gewxezxqv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ggwwvhgik.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gmgcuujsa.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/ggxedwvyk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gqtxbpwla.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gzetoocjr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gvipjgcgt.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/ghbwlebmy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gkqhkjtsj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/grjuqydgd.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/glpsyzaod.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gdzoxvsyw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gwzbytotl.sHtML


<!-- 参考信息 -->