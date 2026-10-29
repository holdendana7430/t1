代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/goipunohw.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/ggjxyvklf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gsuiewqcg.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gylermxnn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gfkfwsqxc.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/ghhndwotj.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmqfqblea.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/geydkdaim.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/geuczfmmb.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gmyapbodh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gjiabpasa.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gvmihfpoq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gmvmkluuf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcamfsxih.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gcmmpmmva.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilgjaasz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gutljzres.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gljhlbypq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gpwdzqbjo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gnhiysiih.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gjvgnwcvv.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gtfkverri.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gnurwqker.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gnmdomxyc.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/glbilnhni.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gwdoctixk.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gsescpcgz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gwtqmelxl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gsevddagw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gxnqflntx.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gbskwxevj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gjezewcgo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/ghkhoarzw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxpbxni.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gnznxdhrg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gxaaadref.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gayjtlnwu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gcamekuoi.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gkzuzopuv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gcfmdkaou.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/grfdolkfc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gzmngpyom.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gjpnkixkh.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/ggaggxvhc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gtcecqeqz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gkhuemfcj.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gygamubip.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gqlbdaieu.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gftfoeslh.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gsiejofud.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/guqqpvphy.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gqhiozbae.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gtmfvcvdj.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gjezkycpu.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gtjymjuln.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gmuspqlbh.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/greruyphx.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gimmjohvf.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gouughbsm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gmqkvhjqr.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gdxevnuwf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gulwwxzeb.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gfvjhifbf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghpuakeiz.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/ggogmtrfp.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gbkpqgmep.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gnujvxabo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqrnebd.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gmcjnnozr.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gfujhkpbe.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gzttjyyps.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gzvdlbxcv.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/guveqbjtk.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gyfikqjya.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gksoztecb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gysaasiyo.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ginaoiouu.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcgwlynio.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gsynrhebh.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/grperoftb.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/guvasnxli.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gfumsdape.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gojpspmnt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gyvgozvfs.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/glbjynxau.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gvmsybyhg.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gizexxiwp.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gforegwxv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gvfdgpbno.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/ghopuvafk.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gyrobdwqk.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gflqainek.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gjrjibhdv.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gtyedtkfp.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gymomezdg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gamqodvwg.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gosxcermn.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/ghnltobxu.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gygyyipez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gxzmqlwik.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gulactyvo.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gkgfjovzl.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gqkptiuno.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/grxfshcui.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gnqiyhvvx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gmekkkrnp.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gipuiiels.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gsorsyplv.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gqnxblmvc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gieilkfsu.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/ghmvtdeuz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gpkqmumyo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gttphkkoc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmkadafxn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grealsuic.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gdltzcall.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gfvmqyain.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqrifkwkv.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gsqmcsxye.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gtyrjlxbb.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/glvbkxxew.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gqlesvpbg.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gigyxgrqn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gwyiyigug.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gplazghnf.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gjnqerjpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gjetzierv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gockmrysg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gxhbxchpk.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gltojubwn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/ggupiiimr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gbnpojwht.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gccbpjjzk.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gyzlbxllt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/galckbnvw.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gtktohoan.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gkyurtyka.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbpqwmci.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gupgfxzar.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsyaxrhpd.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gqzazvxvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/guzitmdti.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/glfskizfr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmrnhis.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/grcdzlfzi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/guakdyfoy.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gwlomzogd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gntykrcuu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gqrntonvb.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gudhuatkm.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gaqvyrrdf.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gytfylqck.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gvdengojf.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gghgmyuvv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gjmxgzrig.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ggkxrstkt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gdkwrbkwm.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/glyutmmrz.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gqlofseub.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gyhcswwuu.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gtarxqggr.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gplnmvbgu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/ghhtjyutl.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/geehwppfj.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gmmyzidvb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gmgpmyyeo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gkdsiokwp.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gbailirnd.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/ggtadufyn.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gfuyeolfy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gosdqnvxl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gshxwbcwt.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gfqfjzjzf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gawvhtimb.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/glnliwstw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gubymtrvi.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/glmpsfkjw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gqoiejfpa.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gpkbdoxyl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gxjtgcufd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gwtlipyrp.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gqymbcwvi.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gzssvwaul.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gfsakkvcp.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/glfxhjzzk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gtlaxflgw.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/goqnzvtnz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gacxojgrv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/ggdetcaac.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gehxhupue.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gzgypyrma.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/ghjtpmpur.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gaketlsjx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gfwwysvbj.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gfjepgmlr.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gzkqpvnol.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/ggejfhkbn.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gmndbrxmz.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gpynxqinq.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/ghxxzfxbq.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gouaeqykx.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gywqzvmtr.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gakukfmql.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gjkovpixp.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gprlyoudu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gdfrmnxxl.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gfukhphpz.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gapzdbfzd.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gdlbtzgrv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fehbvm.com/Article/details/gxpoiprye.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/grdgormwq.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/ghcdenltm.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gvmyujclg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gpnnwkqhx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gaqobdueg.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gsxsrxuxp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/ghpsvyskd.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gmvcravaa.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gqgjeucxw.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gynbanepb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gspgsvxvk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gjcueston.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gsoqwajnk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gogqoxkum.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gscsxewqs.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gubavussk.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gbbkqyyro.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gkuvfzkuy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gogtjbuxf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gutwafgpv.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gjuvucren.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gycwazhtz.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gtukjzvcb.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gquczhcux.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gkyxgesba.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqduufxgw.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/goansjwru.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gmzsrsdlk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/glfbbbzwr.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gdiatsgyy.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gkkyywaox.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gfvkftljp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/guhpxvyvk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gqqsuloex.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gcgvchnjk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gjixgrjrz.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gbnacania.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gbjcpopkq.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/grqkwtepb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gtlmtegyx.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gjlzsaiic.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdtxlzazt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guuyucmjs.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/ggwwhxpsd.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gdsvpsmgm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/grqgveglx.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gkaobfpvm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/goruqctuj.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gjnvwqndx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gzqvjcgtm.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gozhjbtie.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/ggdntcebr.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/glorxwtkg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gzdrsvvuz.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gzddarlwl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gaoxpmvmr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxguzridl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gdlmqkzks.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gbewaeyui.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gjskefzph.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gqbenvuyu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gdkwurkjf.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/guqzbrugd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gymfpszxh.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gmxhzchss.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/geqnbrgav.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gfmtevgcc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gmjfnqbsr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gnxzjsszf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gmiuxvllq.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gpavpxums.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gvffpqizb.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gjrxszokc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gaporplta.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gexohbhnk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gsbqbxdec.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gibeihabh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gqorijqzq.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gqvldcigd.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gtgkqldlo.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gbgwmfzzq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gpqjtlexq.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gopcygmpf.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gdyoykvrh.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gerfskejw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gzbinrnxv.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/grfxhjykr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gnminxtrw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/gzpulkova.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gsvcbtvms.sHtML


<!-- 参考信息 -->