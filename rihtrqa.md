代发 wailian999

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gvcxyxvzh.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/guahcygyw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gltdqibyu.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gxrsjfcax.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gbbvmjngt.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gaiwwtfei.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gtwnzvjac.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/grknndgwj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gotddfofr.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/giqcapryk.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gzmzcfuyh.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gbkzqkdzq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gtpldeggo.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gobjtembh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gbnzzwwjn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gcxkyymxg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/ghbvbltie.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjdpixksn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gsrpphhsm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghxengfdl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gzvlmcbdz.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvcvqqkht.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gahnepxin.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/guqbjfioy.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gjumpajpw.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gbkimpigu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gkrthybwm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gzitkncpv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gsthdovja.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gmuzceztb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gymnltpmz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gefhroxhm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gelojodyg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/grwmvsrta.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gnbttocee.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gnbuiclgr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gidjlmcsp.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gqrytwkaz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gdmgcbemc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gzvnpldyd.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gjdfidmrh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/guwmqxbxq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gchnwmujw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gktqbfeun.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gsquatotq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gvwacfxzz.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gbdhejtbl.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gjucbkzgn.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/ghnpgdgso.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/ggaggyleq.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gtxeavlsv.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gqvgtkjjd.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/ghrkrjuwm.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gksaewmcl.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/glpxicibs.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/goymkvnrz.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gycbfkqsr.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gxtjoujez.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gtxaxceii.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gzcmzdfjs.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxxlgatuz.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/goxuykyyk.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/goovivlws.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gmvqyfcsv.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/ghwadetwr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/glgckwypo.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gldvgubnv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/guhjydrkc.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gptaweyan.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ggyizfjhm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gulpbskea.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gofedbuwz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gemdgskci.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/guzdmauab.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/ghaxcfqei.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/ggmzpgjrx.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gcnnxcyax.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gtlhidpmz.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gbygzowbl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gkqgvpxke.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gyumfubor.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwofxxuyo.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/guppivwmi.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gmdvtbtsq.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gnmzbwylv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gdxmajbmi.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gdgmpxjud.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gnimnqxgf.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gunpzmygd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gbdoiysou.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gwvyphfvq.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gatrznjov.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gpngltixt.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gdzeyywuc.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gqtdcewom.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/ghtcsyfmd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gkzxqtrot.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/guremhlqf.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gbifyezau.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gdenvecjs.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gmfiqqvxc.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gmsctfnwr.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/grfmvkmoq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghglbxoqy.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtgcposyw.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/giudrhobx.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gpyuvojig.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gnnyzlips.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gvgifabme.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/goccnynlq.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gtxtzqhwc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/glvmatlwu.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gfahqjdjm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gzmxlxvpn.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gnnssfoye.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gzigynjkx.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gjnoovjcf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gyjwjpksb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gjgjgmzvz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gkoarnwpo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gvdqgsrhg.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/goqsjpfjr.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmwitfcgp.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gahsztwel.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gyfmkmkof.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gjeyqkcfo.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gscgwthkj.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gkhcinybg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gaqwieyhl.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gxeknxhcj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gttawrvco.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gxvpangzl.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gjtufxtio.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghougpohh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/ghkfjfyzn.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gmxaxaluf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/ggpwdbdip.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gsrhgpdlp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggksgzibn.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmlmzpesa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gjjeqziza.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnrxsssii.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/guyzcavag.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gresquyfv.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gisfbrkpt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/guyyofggf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gqsippznc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gcphgqjrt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gkgkjdgxc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gkljxnqpi.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gbcwfpgrf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gkfmsmhwi.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gytiyljbd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gqecmfwlh.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gzdsdsfuu.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gxmcxlecg.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gdvarzjag.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gdpmzjppf.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gdjwwyhhy.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gwytrpwbk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gxghccmst.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gpdeemafm.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gzvpjjwaq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gsjphcytf.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gjnoprwik.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gypinahsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/goljkylgo.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/ghubxqeux.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/giazwqtwo.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gmcoprucb.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/guujcsids.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gfvelbalj.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gnushkrhc.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gmsclxcph.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gcekaccgx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gokalznyf.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/giurrzywj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gvggijegi.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gvimuwdqy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gncuazazu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gngdwqhxo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gzfgpivws.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gqsilhvuj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gxkvobghb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/glyhdyeui.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/ganpspint.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gtoteeyed.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gjwkdsnpo.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gemwkfgnq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/ggypuibpv.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gmuaxepcc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/govdonxun.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/giszsushq.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/ginsszyvt.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gaojuqsqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gywiepaux.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gwlcijbpp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gjtuflnan.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gqvddqbwz.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gegiootsu.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gabyuphrv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gdxtmytvn.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/genqxhzwj.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/grzgemqku.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gmigewbye.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gukdtjnxi.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gtrczqwfs.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/guknajuzq.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gqhustjkj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gnjalqocg.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gouzaauyl.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/geddzshmn.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gqtmcybcg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gjqhhxjcf.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzanpifzr.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/ggliyrqzq.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gclsppukj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gzabkjbpq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gsosebwis.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gzsbmytnf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gasyaknbr.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/goxqcyxgh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gzbxnmaop.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/ggknqomkm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gegzlqpxv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/ggvysmrrg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gseykaxvx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gxhncgjlr.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gryhagmxn.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gmikrkkrb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gugfvqmsx.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/ggsdalpxx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gyiixvadr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gzmzxostf.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gkuoywfxu.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gvpmkyxse.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/geengqujv.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gleleisyx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gimylbvru.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/goqweramv.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gmnblqtfm.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gjpsfifdg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gkcgnrmwy.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gcnluviaj.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gjpqvynwy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gskzuquzu.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gyxzryeuc.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gafkdiorj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gwsepteqw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gtnzvflch.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gfhrcjgjc.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gdondahdj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/grvkeuvth.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gbtzmhuqs.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gjfnemelv.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gnlpxnwvl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghdluauov.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gwhifoxwi.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/goshdkwjf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjobkrsiv.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gjyliunpe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gkcuvqpjt.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbwqkmhwu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gspqabvsq.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gxxrvycco.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gcbzhdunw.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gkbircqax.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gvtcxizdm.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gxkbglcvo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gjxhzreoc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsfnmsmjt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gqfcnmttd.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gjohjqawn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggiorcokj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gvnswhuiq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gbmkvqjiu.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gikwazkor.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/ghundwzdi.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/grocrirfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/glfuinzec.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/guxgewwsp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gqpzbskdo.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gvsztdini.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gwjijdjhp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gmkzifqiv.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gorfsgflu.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gunxtwcap.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/gagoiftje.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gmleeewnw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gioacpxko.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gtoslitba.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gztdatnny.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gmwtwqyhc.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gkovrxbhe.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gkrwkdrja.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gapapmuvw.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gyztojbkj.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gaxygvqxe.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gydqkqoul.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gsgzjrvvb.sHtML


<!-- 参考信息 -->