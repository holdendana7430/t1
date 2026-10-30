代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gwlzrcyhq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/guivqilhx.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gzzmfomvn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/grzpxhcfa.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gtfrikfmc.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/ghnbkocim.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gqifuvybi.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnotvtmhq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjufesega.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gbreelmzx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gmfwbahoz.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gdgycinsk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gieijfhqg.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/ggaeyxlbk.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gwycycckw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gfkxthcpa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/grxmywdug.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gkoybxtwc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/ggbxtewye.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gfzjgseiz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbwgpibbr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvulskskt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gceghdhyz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsqzljkxj.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grylminmy.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxkelfcqp.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gfgyyaree.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gmfkhlpgm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gpifokcsg.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gdcdikupt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/grthvrfod.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gxnpnsaps.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gyaxkdpqd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gxgbzqyec.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gsafehaaf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtcgqvudw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glvggqpqj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gbkgjlphh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/ggimgtmnw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/ggzscdscf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gzakqropf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gwnpndfhg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/goijdrvoy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/guxzktjoe.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gaxidsdak.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gecxlnztp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gkmpiwwdz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gwmjylhba.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gmhspxkog.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/grgkzufuv.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmuttsnbl.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/goohzmbzs.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gdrshxsqg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gptrjfggw.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gahhktqeg.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghwwnpzck.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gawzgthry.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gohhrxpwe.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gpphgkyan.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gkayhkvie.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gyffbhoff.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gkgtjwgfq.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/grdjzoeft.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/ghwwozjxp.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gvkrpzhdf.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gelvrajou.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/glcotjoxv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gtwwrrlwe.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gglhqfwhz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gwmjbtrzt.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ggavukupa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gnjgqqcfx.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gzdjjnmdd.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gymbjkqbe.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzzcprpzw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gioacpnkc.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gncmqnqdn.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gibciffzo.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/giomqmkrg.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gqsdidnpf.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gmdataliy.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gcfjfygvr.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/giqrtqqut.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gosqnbmks.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gluwjbhtp.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gxmpuzfec.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gxtuvamys.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdgligf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gvhjoptip.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gifeqcdvy.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gerfpgjis.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gsihhpzhw.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gxienbmxu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gcepsrrax.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gtsmerhkg.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gdlfnurka.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/garofqokk.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gxiqwygdb.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gstrkdmie.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ghbzfgavb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/grdshbgzn.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gahhqnunh.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/ghczaqoen.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gabfpqqjt.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkyhxnpju.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gzfirtflf.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gzfxodwwa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gwkcelfbk.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gomwzmccf.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/ghpxfktly.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gzesxaatw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gdefbqfbv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gbrpdyjlz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/ghwxuvyju.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gjxiciwmw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gptlejnrz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gneprepjz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gzbbybdfa.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gxmxccwka.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gpapossis.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gukafynts.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcygpbubr.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/giztcblub.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gqjicwpvm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gtylgsmgc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdliqjtou.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkrocnbub.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/guebfgopu.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ghmexbtdk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzbxntbfw.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/giiyhvche.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gepwesnkw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glokoihrj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/ghopflnri.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gczduxewn.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gxrptbfiy.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gyztpjpuz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gdokdgety.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gkfuqabnc.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gbxtrlwjo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gdbqmjnpo.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gzahsrgzx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gjesozcga.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gjczojnpu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gucimmmtb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtryhcuni.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/guiqtcawl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbqosvusm.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/ghrekekqr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/ggsxpcgou.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/ghkqapsyh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gsuukmvyy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gjbhxcvkf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gtajptief.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gvtchjbzp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gutdvfomz.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gmjpoffjz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsecrzslb.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvmvxhdpv.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gzvkpsvry.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/guqczjdqf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gbvhemmxe.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gcyokfuln.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gtxfauhya.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gtglvqhms.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gwkfmskxw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/giugzkrtj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/ggjaoqnij.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gbjkpxdsx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/goxaudzlp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gsjjqulke.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gzcmjiggn.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/ggjrwpqjg.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gkfhuqrpr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gmsixdsqz.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/giyvdqifi.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gtxillvbv.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gtplzgzwx.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/giztyzvfq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gohjbbjkp.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gvwjdozpe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gnbmstnzm.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gomihpmcj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gztlqtpus.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gthweofrb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/glxuxjjlp.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/glavkwnlk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gsgkxxcyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gllzepzzj.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gkgbmzzxy.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gcwtcnrev.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gxkdpuxjw.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gqddhbhbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gfwytzpig.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gquzlqifg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gqxcbleng.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gwjwsaqhq.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gicrbnmhe.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/glcjvgosj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/ghiimswsz.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gxtgmasbr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gvpmvksrn.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gjypayzdq.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/grgmjnpbg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gzldwqqdg.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gicogxhgl.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gbinmyesb.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/goewfkwqu.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gbwxalwsj.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gyhkdlrui.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gppbltpuk.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gembaahts.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gxyntjwnw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/ggadgxbvf.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gdssktqwt.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gypprqxkw.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gzxnzsjjp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gzsgspsdg.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gpjdnebya.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gwpgrwlfq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gfshclqny.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/ghcrcdwwc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gxgltodcq.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gspkysdzx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/ggtipkebn.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/ggsuznsux.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/goxcnixtf.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gvzqbbwmf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/giuyjtdfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gpkzbeywb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/grdcuyeun.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gsqlnljtg.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/ggsyqwfdl.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/glpmfcjon.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gaukigxaw.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gqmrggpcj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gxkxkeclt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gfetecbiu.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gbrufitzb.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/ghcowsqvt.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/grcehzcvb.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gyfruputk.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gdiwzfboq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/garcdixyy.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gpqwuhmrs.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gkiztilwn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gztmygxqp.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gqdogrvri.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/ggrfmvtmt.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gcwntbmwa.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbqkyjhnv.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gfggcypbr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gvtsuuzfa.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gpmyywsmt.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/geogqrsya.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gqalsgpex.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gatkohfbs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/grfxzdlmk.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gpmeamkuw.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gopjlathc.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/guqkniuia.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gpqnqqqib.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gkloaohae.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxkceqybz.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gitdlmqiz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gdejbswql.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/geyjgyqpg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gpsdcaqio.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/godtkyeph.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/goyhrukkr.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gndemgahu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gvqdcrtli.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/galpiqpxm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gginikrwb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gnrjnfmpr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gevrlrugf.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/galghksib.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsbvdown.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gpwxpsvdw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gzgkrxcod.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gdujzfghj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gazquypqs.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/guvufrmjf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gxtdrprvt.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gkblsibpe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gqlmflzyl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gusjvvckk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gcjilvola.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gkhajyizw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/ggagtkpyc.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gehymnrbp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gaggljhnw.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gxjhplwex.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/grkmseryr.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqdjtanid.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gwhutdlpy.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gkllyadgo.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gvkggapux.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gncobqmin.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gdiifihhj.sHtML


<!-- 参考信息 -->