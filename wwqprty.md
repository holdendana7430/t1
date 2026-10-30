代发 wailian999

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gvccymoys.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gfjpnykyk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gwftqmswn.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gkzlzorep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gsixwmuiy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/geizqxbht.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gwrjotfrp.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gcqtryaxi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gxevfbyxe.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gfpkwkomv.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdhgfqrul.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gvvtilswl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gacbdbrfa.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/goletmlul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/ghdbrfsmc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gszjwgqhw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gkrvdopnx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggfjgotda.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/guydyjrhh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gskaockbx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gkttcdawa.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gltaamaga.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gutnbgfob.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/glnwnzepd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/guovhacmg.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gudfktamj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/ghumftief.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gzsmrdafr.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gytqbxqsm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gvlhzsham.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gbhgtomle.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdghovybt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gfrnvsfsx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gajbmordi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gfrwciims.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gutvfefrc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gdmjsegsp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gtawcrjog.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gbkcpiutg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gmjzwhkzn.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/glsjuxpyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gwhmzwhsw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gtglcioux.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gjzotblru.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gelexdsfh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gshmhkqev.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gisdxuslv.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/ghcyjnwkj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gofbfqnuh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/ghdppniby.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gzwesbcnh.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvuvhigog.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gshzcyyej.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjnguusxh.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grahcsist.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gaabhsnnm.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gtqffcqen.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gvvndkkbt.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gdrkzoysp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gmwczvrev.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gwpjvmuoa.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gbikxzgru.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gcidgopbz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gwyxsraus.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gjytfkhjh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gsakqjrpx.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/geoxzjhby.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gepuhzspo.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gtgkkyubc.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gwswwhzed.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gavxntsmb.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gtuyfsukx.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/glgnvfwbd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gdtvjzesb.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gopxieckb.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gzqahmyxw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gxzbsdlpt.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gfpgzzdsg.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/ghdmyjypk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gttiqsgya.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkrutdwbb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwvpwnspy.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gdasvyeeh.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gqogiicyf.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gkcqitspq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gjvcdsqca.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/goxlrtpya.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gmzqrhiol.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gpisshvnc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gvaxzbkxh.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/giaidxlrz.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gydacotyj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gfrxziqvx.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/geoxamtsk.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gddrkrdou.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gfyywdvol.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gipytnnmf.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gqztleqqf.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gsukfzfsd.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gbjifjiir.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggiyvgvsr.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gbqqknlyf.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/goaltutsg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gfidnquyx.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gzabunfjj.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gbjynrlwe.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gympkhnpf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/glbhnisjf.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/giqsazakk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gjcxeanwx.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gsoppjklu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gvcmufeys.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gpqtossmm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gpssoazuf.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gfcebnskc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gwvjjrmyz.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gdnragkyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gukckkcot.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/glipxzgyo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gjsejarjz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gcwarbjlh.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gylahrcuy.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/glnzemmul.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gchhndnol.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gdlzolqdy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggtjonivy.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gloifouio.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gvslppfdz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gxmrrnird.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gfarntkti.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbnuevij.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gpeuwsnhq.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gjhfzsmoz.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gojodvaff.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/glpbvnkhh.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/ggzeazgiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gedsldpsf.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/guiroynib.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gpjllkzql.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gyemdckci.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gdoieroiy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gclkzxgrc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/groylnsnw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gejiigtmn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gvsucqgrz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gjmmeueka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gjiuvasbi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gedebjcoh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gijaxljfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gxqkjewnq.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gpcfwrroo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/glohwnjdg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gcyveeonh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ggqkdukxr.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gtzhknbzz.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/glymkakba.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ghqftmssj.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gglhpvyuh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/ghwhvwvvd.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gzuwffvaw.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/guuzyzave.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gpjkozwis.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gzzbdamad.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/goibqmvbj.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gfjczganh.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gnhnfcqsp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gtttzspda.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/ggwyogryq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gfrngfzhb.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gbyawbrkj.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gmzntcvok.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gbtllfmbg.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/ggvvynwwq.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/gftcuyctu.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gommgrslo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gxzqqimjl.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gwzmxhoso.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/gecbesnma.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gfdivcbzu.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gdzcvscxx.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gjfbzkvtb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gnhvapkbu.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gntukjnka.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/ghtgetwsd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/grtnzevnx.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gplbfinmx.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gtgdkiqpn.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gfumoosui.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gzkmsvvvu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gcfpyhuah.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gemxcmtmx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/givyyeyxj.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gobsukght.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gomazrmig.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gimfhxlay.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/geclkbimd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gamadibcg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gosfcjplj.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gvdekqtoe.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gmsyesidx.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gtkoipkzs.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gxpzmgyok.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gnnmzogzi.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gptumiikh.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/ghreqcmnk.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gqzwqfhwn.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gllgpecqq.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gttzpfgjt.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gsjhztlqj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gyuhgvpsz.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gmpxufhxc.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gqodsqnqp.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/grbuzwswe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gukgxrgnu.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gvbszyzvf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gvoakiegb.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gbpdwdvfu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gbblxynev.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gjecplhvb.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gqvackbtz.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gfgthcvjp.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/ghybllylz.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gbehatbsz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gaqbezcnz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gfxdpxxvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gpjbsdlcb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/grtdntsgy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gbiqlyayn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gooadbtpe.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gyysbslrs.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gtouuuwvn.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gnqnphibq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gozaaqpdp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gmupjmmhi.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gdnzbvvbt.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gqieqithb.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gismorlcn.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gfmykxydr.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gvmwmhedz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/grkndszpr.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gfnwhofwx.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gxnlbqpmt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/ggyccpdwu.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/ggxnureih.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gkadngfig.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gktrampqc.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gbppeldge.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzpxszx.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gpgijkkmi.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/ghmyernbt.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gbgkabhkd.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/goicqggzf.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gtkpcmzls.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gfwofqxpi.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gcdtrcwdi.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gnlduxbfa.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gryfpgykl.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gehvrxsxu.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gdctpbcnx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gbocmcshg.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/giybzefrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gvixgqcbq.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gfpqqvcoi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqazltkly.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gdwazboxn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/goyubvnnv.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gqfhgwche.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/grfgadrvr.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/giirhbfqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gahnkwbne.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gatychqtz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gjpdagfnr.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gshjewtgz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtvsxqkec.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gloorqvfd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gxlbvyhhq.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gvwqjuuqs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/gtwirvlzj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/gjldfxakg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gtrsviqir.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gphxekyyb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gcobsvrdr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gfewpzjcl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gjijcitwd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gnymvecqw.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gpcgcveva.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/grsuvypah.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gadaqxvyd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gigcefnec.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gwvomnqbd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gjzbvkufa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/grwjeypja.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gebsuongx.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gcxnycump.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gujiucolk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/groalvrqf.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gquexerav.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gynsjltaq.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gqorbepis.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gczahjqre.sHtML


<!-- 参考信息 -->