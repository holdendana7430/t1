代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gzgpaxplf.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gpxspdoii.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/ghetnouee.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gbnfrthoy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/guqamlasf.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gdnvcqvdl.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gdezcohri.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gbzqijoax.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gezbysmma.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gnnrmnpte.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/ggdzmrbki.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gpfaxoizv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/goauvzbhu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmabizexl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/geemqnkha.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwqsgcfgy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gvzavlpue.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gdsbkmvoi.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gjgdnobsb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gciqottzm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gsuptpiwr.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqdgqqkep.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gxifsvdkc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/guqhfddnv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gtsswpflz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/guhdzmmbd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmqodarol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpynnnzyk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gdmwxbvsx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gkneskoqu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/ghltriljb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gvmqhheyp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gpviwsnek.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gyvbhkoiu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gtskkfdia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gvyvozngr.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gxairchtd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gccpmugva.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gwlhcntid.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtrnxwmod.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gzcppwcaf.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gibevgzuq.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gvnmbyqoh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/glcnlzsyf.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/grmraribf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gabbhvcpn.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gyqzkmjti.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gijjwokgz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gkxpmnqgm.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwfalhzvp.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grzhsqrfr.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ggvearlrj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gmwsayerr.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gmvwoiajc.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gwgpxdblp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gghxeowxu.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/ghpbewyla.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gcjswapge.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gnmvjpdyx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gggfssihr.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gywvmxldb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gzgufhgwj.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gxaegnugl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/grzpkyoro.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gsubqunxf.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gyqchggzm.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/glrsaadzj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gqoxjihus.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/guvwuxgsp.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/glgdkmvnk.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gbmhofoxj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gorbjnqba.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gtwbfwesf.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gtbdpjerb.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gacthdixn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/goegiubjb.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnlupfpgy.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gznzvfduz.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gtgdyjszz.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/grhlolduk.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gnuzjzarm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gbvnznotr.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/ggtgtyxea.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gowruqsjj.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gvhhaftlj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/goecsyfwd.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmpqwrbrz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gbktmvimw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmdwviidw.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gaykkxfhe.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gxudkqwsb.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gguqmtixc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gltkyvvib.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gajscaljd.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gfqvwndkz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/grnedwyks.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtopgqyon.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gxloyhenu.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gtldegtig.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/ggvkxauyy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/glyljtjbv.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gcyffwoct.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gioaobwtv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gleiaqlsn.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/glfeuwunq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gzfpvzlad.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gsfgrzhfp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gcqnjseff.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gtbpyudpq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gmvfrjryd.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gklffsrmi.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gzdrotsxg.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gnnkoyzgm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gnmzxlvkj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwpfevfvi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gnhivstrx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gekqeswef.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfacwocqe.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ghwnfatyb.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gxanfbsjg.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gbcqchxvf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gctgjoptd.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gbtijydur.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gawllmifk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gxjzonqze.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gxjcdjatw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gigibhcwa.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gjmgjkjrm.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gjmbghvxy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guukhkuec.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gzqzuusqv.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gnmmtueoj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gxisoaimo.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gmzylmrat.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gcptrfeue.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gqxojjzwi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gvlcczjck.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsabdalwb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxqjakena.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmeymsaeq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gskzxjfbq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gdlcrajpi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gaypoexsg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gzfaisqie.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gvfutyutz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gvaywwwqy.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gsxiyuxff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gttudcjnt.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gzkredaco.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyefxzghq.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gihnkzjbd.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gwwapzylf.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gvyepdfwl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gcmzhmfyk.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/glewphegr.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gnzayqcbk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gzemvzqhk.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/geerubavf.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gorgdness.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gdkuslaaf.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gbgrwuyhj.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gnfcxexvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gxjpfnihv.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gqxnlffba.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gxrgjuorf.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/goecijonf.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gofedqiqo.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gvuvxugfr.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/glwrevhsk.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gexaaiqkv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gzwmgvztn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gybbelalv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gmfdrshxm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gozprwuhz.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gtgjuzbai.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gsmepsmpe.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gvpwlusro.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/ghbmrzxec.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gqlgdgjlw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/glgzdvtkk.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gazwuqsmu.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gtyutnfen.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gqohdpbqg.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gejfwbwbb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gwcgvefjq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gurdqddvr.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gapexfddg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gpwzcdpki.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/grgsrwwap.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gcncfsugf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/grxbgqtrs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/glfhjyldq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gflhffbws.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gjjcypzrm.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gagtiesmv.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gcfzttgtd.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gomlwuylp.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/ggmltzsbh.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gfrymqghg.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gbrepdcin.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gyfuhgxvr.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gpgaiqunx.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gvxpmtafs.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gxxibusja.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gqmeaenor.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gwdrcgnxw.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gypehbiak.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gggnrknsl.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/grfqolude.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gfbfhtoxm.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/givfgojai.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gdkkfadnf.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gbfuxdbkd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gevrcqlxg.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/glgchaclk.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gfotwiqnd.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/ginyqytwj.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gyclgensu.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gtuciqccl.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/goixpwuby.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gabmnrdwq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gitvifoyx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gmswlxeam.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gqpuudgvp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/greugpqax.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gtkblykmu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gzntyidgh.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gvpdlqzjx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gczgwyzwp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gnbgaedsm.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/ginoamcnv.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gdzhokfsk.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gkxdbiryh.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/glbpugmcl.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gowqclrgm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gcnreogdi.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gziuyxuix.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gobqyxmbh.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gywwxbsjv.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gucepkfih.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gatqgulmy.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gyxnyqrnv.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gachjvzec.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gavebvsvt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/genzbeewd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gzhlkiwvk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gymareuey.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gsgavuzuu.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/ggmlplomd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjsohtxfo.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/grafwvoej.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gpaomvmku.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gptadyukv.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/ggjjvekgz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gxewflzsd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gnztyjohy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gegfikran.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gankcbqon.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gbhtfboqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gxlxhxzsv.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gxdpwyfxe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gfqadabpy.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gtjzythrd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/giwteowqm.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gsqtiinyr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gfqroulki.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/girfwdpdy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/goibkxcgu.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gpjwglmsx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gatampvoa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gvbtnvhko.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/ghourclzm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gsuhahyql.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/goztsiomp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gfmhgbftp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/giubruscz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gyrcqbvdz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gucproxjw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gwtahfhuc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/ggwfktyoj.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gyzmzrfla.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gwdamxxri.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gmaxxgkjp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gxslgsdso.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gqxtkxjbl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gnomepdef.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gsbunjixr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gjfmadyyk.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/goxlhdxbh.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gcwehkumm.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gfeixgern.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gzjvqdixe.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gjazkrzol.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gpbfotttt.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gegyenpod.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gtowzwbaf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gzdrcezod.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/glqdnfkkh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gnfabnpka.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gycinspdm.sHtML


<!-- 参考信息 -->