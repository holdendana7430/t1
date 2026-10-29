代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjvurceou.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gqbiydtkq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gmcniivwt.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gadwgtuex.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/giaiapkmy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gdodlfwxq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gftahqrnv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/glptbdiav.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gemjbtdhb.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gfwpnlbep.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gxjrhxdmx.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gbjrhgcsu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gejeaxrab.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/ggeltytui.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gsxdoajeq.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gmczpasfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/ghukhgobk.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/glbioqwlv.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfwqgltwi.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gouidlnht.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gcqqoepml.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gdfgsdhbf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gsyzbsttc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gzmcrlljh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gawleqhzs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsixucnji.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gyfdjvbma.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gostecuzi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqqfdogxa.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmycxdwqp.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gzssrzrdq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gdwdyhlxz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gsrlepfif.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gmtkckhoi.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/grmnwacld.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gwqhqwfhj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/glwlbbnbc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gzhjzwstu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ghjcrbgom.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghszyezly.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gphqzmbng.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/glsxvijpu.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gcfsylyjf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gavrpriab.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gehnxnqpd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gwkriosfo.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gxfordibs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gvmqbeizq.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/grwmprzhh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gsbkfepbt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/ggtyxulkb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gfdvrelil.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/geoxwpfbl.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/githojysy.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gogcdfugg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gzgtdsygv.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gdhyslpdx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gepwvftzd.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gdycnwozz.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxqglyagm.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gfhtfcdlp.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gtokuysys.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbvmtmlov.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gmybadspm.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gcjjwqttn.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gvlzobpmi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpwvpbb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/ggdpfdxst.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcebscnpl.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gizhroxpm.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gldvikwcx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmdlajfpa.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gqfrekqzv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gvvvndbtp.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/giofekbuu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/grnheusge.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gohehijfi.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gtbpphtvm.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gwcvmorqv.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gfhnoktgw.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gfwqlgjwr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gmqwcshwf.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/getggxfyy.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gjiojqwfw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gsscuhscg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gewwmdkwp.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gdlyddrgj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gqwcswdod.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkimwvdeg.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxpipkssr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/glpwidifm.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gbpigdmaa.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/ggpiejhzb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/geyeoitjj.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gzrmkccbl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gkfulaiev.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/genovgrmk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ggskpjdio.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gaczejfzk.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gubeneace.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmmtvffua.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ggfptaeul.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gdzpcjlqf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gkzcsegmz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gbyqtbozw.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gmjxzifgp.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gwqiratla.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gfgvgpges.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/grcolahdq.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/ggjpljsqg.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gpcuszfbi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/ginqvyayz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gfiarpowt.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gzrgklfxs.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gzxzncvtt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/giyepxgww.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gwzdsolvq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gpfxmrcoj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gjcvqxkjs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gujjbhvzi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gvwsxpxha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gfnzbskfe.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/giheezylh.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gtnpwjykv.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gxjxffalw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmgzguijx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gutrekace.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gkxunqjrj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gvafocreq.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmcdaolgg.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gdazhnusv.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gandfjezk.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gxnaqvqxs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwmzrjpna.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gdxdpesxi.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gtwnenaol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gfozdifdk.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gnztuvgec.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gscmnvxkx.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/ggwzbsxav.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gkmmkhvmg.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/giatmndkx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gtretpdrr.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gnlskyvok.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gfquidgwq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gxjqkwvzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gytjxdklu.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gcezlzzaj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/goffanwum.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfvpuotpu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gyqbhovpj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxemhknup.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gdnijolqe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gkvmjwtpi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gbnbmpljt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/grvsiiogc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gsvugtzcs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gelwsrmyo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gdhdepxcc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/guhhdistq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gnxbqemaa.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ginrwstej.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ghkfilusv.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gpfbcptcz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gckkowavk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gsmixkkbi.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gwwshijtn.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gvadlfbwb.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gxnaudcvc.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/goqgwgmkn.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gjjzxtxfc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gykeqahlf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gwpzqjbyv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gbjrxjbzu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gfjgrrhri.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/ghtcpqceq.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gelvwkads.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/ghwpgjxiw.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gvtmaicpd.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gcjqtneru.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gykllxaqq.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/glshgrzcp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gjeywbxbd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/goztnqkqg.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gwqklqvms.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/geekgquxg.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gwwbmcgxq.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gudzddmsl.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gtzkrhpvr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gbtekdttn.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gxlhkhmjr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gpywograk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gpruobpug.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gguioyrvs.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gggeyuauh.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gzyelkbwf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gwjztewfd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gubwewfmh.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gbldwqdyp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gynnhfgnj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gersftehs.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gftmxsyzo.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gktuxdnxh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/guujhxktr.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/glwqsizei.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gmxsgqfvr.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwffsnlta.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gxmplngta.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gpkpfnhdg.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gasybwmmh.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gvswseysn.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gkpiedmll.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/graacfkme.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gaskvnimb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gcovabdpv.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gszgyflhh.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/ggymtthsr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gpwogindo.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gnvfhqrhl.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gatkfxcod.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gatkwxsyq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gcgtnpayp.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gisyyupze.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gweyudjws.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gzqflbvem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gxsnmhuth.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gjfnlcpzz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gxxweyuuo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gojgswwwv.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/giosbckrf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/grumgmgtx.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gxwctnxsv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gqyzmouwl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/golaflpnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gyjvoqyzz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gxezzuwbg.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gvbtlzcnc.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gcxvyohlh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gbsnciwyq.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/ghalhvnnv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gpqfkddhf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ghbcmbcct.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gtywepqhv.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gvymahanr.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gskpyswsn.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gnhoznwjo.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gzhuxsxiy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdcfjlwol.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gfkwlfvlx.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gcvfbfkml.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gxyzfbaou.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gfsqpeoif.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gxrtskhbq.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gvvrecxpj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/goduyifbs.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gywvutpgw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gtilqrkyx.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gwnaefcpc.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gbbznultb.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gfjkughlq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gmdascuyx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gogbfhadv.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/glkeidiwc.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gttcdsqdn.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/grkscpqti.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gxlhbhvqh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gksolwoma.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gbmpyxxrq.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gycwsbrfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gnficflqj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gywoqtofb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gkmgaysut.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gzfiaidti.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfhwevkkt.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gfaiwbxmm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/geqelcsqq.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gponkrnbn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gbiyschgd.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gmvfqnmxv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gmjqzjlqy.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gfspbljjt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gdibnxwdy.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/ghkopevmq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/ghmgakodz.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gcbevheax.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gmdzisjbq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gvxstnijs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gjsoxajrk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gintpxogc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/grhrswfbc.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gguttfydl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gffbfpjhl.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gialiybuw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/grgikmgvh.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gafrjpype.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gxlgiigyi.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gannsqlkr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gitdzowad.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gmxdjvqzj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gvcydujzz.sHtML


<!-- 参考信息 -->