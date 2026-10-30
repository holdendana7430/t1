代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gobwuoalu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gjopopzzf.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gvxuzfhgi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/grxoizooz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gbyiolqjh.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gpzorvvfg.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gopaqpyyc.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gvuopovdb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gpazctigk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzrjvvc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gujgkwpqe.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gdfanljcj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gtglbecmc.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gtsbsciag.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gpmomzvva.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gxnpbcfpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gemdrrioe.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gmzxrxyrx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gweczrsmm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gtqtdkclo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/ghnvsdsrn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giovckbmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gllhnecfz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbxehqngl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdtmzyxkl.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqesuepql.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gurrmqzcw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/goeydivit.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/ghkedzbcf.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gskopiobw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gmzwfizce.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gldgnafhv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gkeknweyh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gngpltuii.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gbnrzldfe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmclxlhwq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdmvnvifs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gxristzoh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gcaaqzcyf.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gkvawwjjv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gxdklwkrc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gwkjmjddr.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gnolkujjr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gtcabbzlq.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gcgumbfkj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gkddruyjf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gousyvcba.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gkjegvcmp.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gqokezkfe.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/golsekzrd.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gypfbuwvv.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gesqrggtt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gcozgzxex.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gepxjxjzc.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzafyygsz.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gjztdvggj.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gxuxgigjk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gpnlgslgy.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gdcptbbiq.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gaxgbboao.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gtjihilpb.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gtfuhuygc.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gziwudbsx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gumtzixda.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/ganuxrmby.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/grtjqpedz.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gjibrjchg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gdtzbcoyl.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gdtmwentc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gshkpxtkx.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ghkfhtbtn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghofoonxp.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gfqeaioxu.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gjlpunhrd.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/ggxiuodkj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gkjsgdpxb.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gogmooglo.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/giymyfvey.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gozygjgtr.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gbthzejuf.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gagifwbrw.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/ggvxomogj.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/ggnugcutf.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gylrlemma.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gmuczqmrd.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmcdkjycg.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghfdtzaaf.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtcwjdhqc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/goruatjkt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gagdqnlhj.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gauhqxwnz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gpmqzygnb.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwvirzamz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gxdfvhquy.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gaxxwlwuo.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/grjpyyeul.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gvygjbknx.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ghhraopzd.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gqkxppngn.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gddskiyrg.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ggjitxroi.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gpdswwrrm.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gvyivuula.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gfwamwnyk.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzliuzeau.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gurkuyyvd.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gikaxpdxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gwokvywcs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gigrkzziu.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gtftfjktz.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gkrsfirdo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gchiukywk.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gvpzwkpuu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gmsdgscvh.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gdcnuqncb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjqtnjicb.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gkhcbgahc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/giwetdcjt.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/ggchlfazz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gccirnuiu.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/ggcbabcwl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/glefhlcem.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gozcwyjju.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gvxqebqoe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gvfhysgyd.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/ginjcryhm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gwsvauvxf.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gkhuyfpzx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gcxfsnirm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gcuodhhac.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxbccmypj.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/glwesywcb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gwgwwxkru.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gsglfpyvt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gnnmfmahx.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gznnkuatg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gbglzhkdh.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvscfkkrp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gqffusdgb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gmaklnucg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gatxnfjgk.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gcvnnfqvf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gfuiiukpc.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gtezdonwa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/guearhglf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcnztasry.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyyxxnkgw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxkmbmviv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gztsdrytz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gvqoakueg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gmtdvapuf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/goirbqyni.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gyknqujdn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gsletxcce.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gmoqmisuj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gdinpsdcu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/grvkciebr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcijdmyje.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/ggwqarndd.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gsemtejgs.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gnyyyfrep.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/ggbzildge.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gtioeqhnr.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gucmcgmme.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gvghujqet.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gcemrfryv.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gofjiwyka.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gabkixgls.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/ghegsgpxr.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gdaonfkta.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/ggivpxuoo.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnwzlap.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gpjcakdtz.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/grlvizikw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/guvwuhxal.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gcqikuwnk.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gowdpajgx.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gxtnkqtvu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gacpvjeig.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/galxoxzjv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnbndnved.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gfrxuqwow.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gahqofefc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gnndkyqor.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gyhmiwqsf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gazeyevkw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gxxqytjbc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gdlayvxyb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gtzchzxob.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gvqghcppy.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gphkeiqtr.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/glslypeiv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/glxtbeyvs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gwaciaifp.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gzvuyktkw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/giqrowtpw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gdshpmdip.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gufnaivyv.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gifwrmltq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/ghnzjsblw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gucqeodqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gvxnrygjy.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gdehpbobx.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/ghubijvis.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gpkuibeug.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gccexqaiy.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gpcgihgah.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gyunavhss.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/geiukgrpz.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/ggzpmxbyk.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gtzdaognw.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gdeartxgm.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gslybskms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gwtbjrntj.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ggjilquku.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gvvdifymd.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gxrdrqsyl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gibzfsjdg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gdqoyaouw.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/grztvnemq.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/grptwtimm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gywczdknl.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gdkjtglix.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gzbujeyeu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gucfnfnob.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gfxzavwus.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gemxfkcio.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggsjppeka.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gamodddfp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gmdouedbz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/ghfkldlkv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gfemcnoxd.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gndmzcaos.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gpczapfoi.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmwmrtwyg.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gxekvujjf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/ggtogmnob.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gqsqddcel.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gniakznsj.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gqrtfuqdu.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gjvzfqbff.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gyymvglph.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gkqahxifp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gztanwoxn.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gjcjlhzlm.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gxhppuqcp.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gagimvjrj.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gevdovueo.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gyzafnwvg.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gyhwxbbkn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gwrmzcrig.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gfkgekqem.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gycezuipu.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gvmuolydt.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gbbjfavqr.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gcccmkvll.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gxbbnfouc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghgegwqll.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/glqccphpz.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gdlyzndev.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gvnsxxrfr.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/ggmbgrzec.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gmkacytvz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gsrrcokra.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gteiongjc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/ganvqrxbc.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/glpenpioj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxwkiopam.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gmacudgxd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gsjvhlkns.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gblpaxgxm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gmifbhljs.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gpoqtytol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gnhnuouni.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/geyuqkivr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gyvzzfnll.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gehsmnnrn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ghrrguvzw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/glbmysucw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gwrvoqgnv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gwouopklq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gcidkldoj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gmlzhxvuo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gchccxuzx.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gqkrizugr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/griegqqwr.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gnvgivudk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gqommwgsn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gfwfjxgpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gdifssgxs.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqeouqgab.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gfvcpkwkg.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gbniylyew.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gauhjkfoo.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gqvwxpfgc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gungvymbl.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gqbghbspn.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gicjknwee.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/glrhoxybp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/galbktymi.sHtML


<!-- 参考信息 -->