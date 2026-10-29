代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghwyqwrli.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gjpymoyfw.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gevtjsijy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gmojeukye.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gqcanivkg.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gbgwgzwnv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtxteupj.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/ghwcqkibr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gozkdrdbk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/giwnviwlx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gojpwtumz.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/glefreeas.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gllzwiott.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gpzdcnnri.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gdelgblsm.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/govfcwvji.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gpgrkoody.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/grtdddxsf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/glqpiqmgm.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gpubnglte.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gefqredwl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkpjemluo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/giuiqzhqi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqepedvom.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gccrfwjws.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gysmjayxj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gahekvhkt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gdodgtgka.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gmcxszvxr.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gbhgjfwuu.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gvyhydzvq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxxhoybdu.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gwnjmfrxk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gortsirmp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/geofnnkyh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gvockxfha.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gfqiafqfp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/guckhdkdb.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gjruddrzw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gyqynrums.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gikizrrlx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/goqxzfiyx.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmkzmmcbq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gvpjkbgcn.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gjvkhcwsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gozdmhbxl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/giigmswzq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/ghbfrewyi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gxvovcisn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbvmradzd.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gdokkabze.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmojoeicj.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gwuqwjqwr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/geawovaol.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdqhpomst.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvsdokben.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gleczxdcl.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gazagqprb.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqdooipjv.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gsypznmvh.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gybwjfgqx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gkopfhspf.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gwjuthcjc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gfnclvslp.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ggoctoxam.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gigqzaxhj.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gadgsdwjt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gwomdbhzc.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gpieloajy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/ghxvopkhi.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gsfsvddbs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwymsvpdy.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gvkixatqm.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gzhjhzvtx.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gjhbjsyws.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gsntcczdx.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gvsbaneyn.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gaszhnthr.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gehwrcpnj.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gjiduezwp.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/grwadjcob.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gwogfjrnl.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/grhwcuukz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gwmhqcwld.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvuwjhnzr.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvvmxhutz.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gdsobjddb.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzfsdjgkg.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/ghpfomvai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gupmpanfg.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gfurtwhjg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gmuevvgrn.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gezlezzwp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/grgngeted.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/grlnpowwt.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gzzxlknpy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gfhkoyqfm.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gsmoaolbp.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjkjhbkfi.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxitmtxox.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gfpqyswvl.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gpczeofnz.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gblouklgo.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/ginvxdvky.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gijpnuxrw.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/goisrbtsq.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gzalrmjls.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/ggokvgvfe.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/grwveyire.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gzilltgtd.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gvnfzapos.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gwzwixzbt.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/ghqvelnle.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/ggczcctit.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gtdidetxr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gtyklopup.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gyuoviajl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gjutqmsxy.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/goufjcnum.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gohkslovu.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gteezcyxi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gyieiszxk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gvddjrviv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/ggmffdlzy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gqxgvvhis.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpjrortmj.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpuvrczcp.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gmhwylrgt.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gugobfpvg.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmxqqiqbq.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gyzafvces.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gpekspqos.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gpimhzczh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gkvornfas.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gpempfxcl.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gntjnkndt.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gddenwdes.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gljtexvop.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gdblaullk.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/grdoeypqr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gbdiwxljj.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gwwbewexu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcmwssx.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gibfpaigu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gwalcfevq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gufeaqskz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ghcljkvkh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grocgpmwx.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gesqknczk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gtnkwvgkg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gogoryelz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwbeahghu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gpfxppjnz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gchzufnqf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gvxyrejrt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gxuehcvcw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gclapkzbv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gxhulxihi.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gkxuwkunn.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gflmjgzbl.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/ggdsccvcj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gbdhijfpu.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gtdbonred.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gdelixjxl.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gzisxxbeb.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gxcmgxtrf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gkuaoujqu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gcjolshju.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gfxxtmnbk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gyhipuisy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gafqtwdwu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/goqahiena.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/ggkpnbyhg.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gizenkmtk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gbalfskgt.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/grijauesq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gpcxvqrvi.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/glligwoln.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gtppyrxlq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gvrgctfkj.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gumihhbhq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gcrhrohoi.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gnucpxhnx.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/grqcpploi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/glwisdhzp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gqqcbjhtk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gsnalolnj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gujkzwuoa.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gwrqdzsym.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/ghqcotqgb.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gieuvowcb.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gdkpnomrh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gxwyxdyau.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gfecqghjh.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gqdvihcjd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gmtxdvjwt.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gtkapztoi.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gpifmeprt.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/ghmnctsha.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/glmaavsfv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gaepeimja.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gaxrnvdke.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gtntrondd.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gtveokjyx.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/glasptlvy.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/goryntwiy.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gcchtfkuq.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gtfaexrzw.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gciyboxrt.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gwdjezrkt.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gymqrqcbp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gkwklxgpu.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gfnirlnvm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/guagqinpf.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gensqzsjx.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdamruiu.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gqbieonhd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gvtfubjal.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gflweespp.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gcgjqduic.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gaatsmtjv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gixfunodr.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gnfuybwvl.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gqbcogovs.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gdknvoqju.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/ggsovblrj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gqvsahdvt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gwsjwrckf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gigckovyr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/ghjvpwsbb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gqgvxkofr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/ghwvplscs.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gwkubrtjt.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/glrndogps.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gnbruzkkg.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gumiiqevq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/giwapxqps.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/geoffvdql.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/ghpfaucgh.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gakssxqfq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gajybjivq.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gificgjej.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gbuwvszlb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumqwxyhz.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gwjvyfrgf.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gcoaenopx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gnfbwgggy.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbfuycbrk.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gzcmepsqq.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gemfesoya.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gobyskuay.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gtmadwzks.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gpdmucknp.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gyprvffrj.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gmfgfpetm.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gmcxdprwm.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/glcxvyoiv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gkoegngbw.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gujjfyatl.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gkatorewp.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gteqwjwui.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gnxvkpjbp.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gmfwugbbf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gcilpxyvl.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gkusdosry.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/grzfrbzcd.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gdmzbmemt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gjtgtkbqm.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/glqohaytp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gqaoyvtbw.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gwzgehhzp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/ghcphkhxx.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/griiwodrz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gthkswovr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gjqlmceuf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ghyicgvfx.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gagovmsnz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxftdhsrc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gezlphjby.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gkjjdifvd.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/ghahmgqcz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gxyfxtxlc.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gpoafurqv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gcwqqhhts.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gjpmenyam.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gonrvhrmi.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gdgttpanm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gykaqvnxz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gbuevjpts.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gqhdpllvi.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/glkpiktkv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gffcsmhuw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/grfctpnfi.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gbvbuhtnv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gwtfsflbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gywlcunwg.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/ggwibscxb.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gfzwozjyk.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gzlpsyodw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gwdtqtyvf.sHtML


<!-- 参考信息 -->