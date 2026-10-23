代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dmvthxkh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gnpvzfpw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nwqyvywi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pmyxogel.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3suhmupgm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fhsfgyws.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hypokzgw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bvpizjvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxjdliuy.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xaphgopq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zylcifcb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sdkndqtn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rreninlp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3doxszlpc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cbmdabji.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqhhdbiq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3phzgzbct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmwyruzf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uabcntnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkvtdovt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gphkjdzr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3genxpieg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bpujqxqv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jzipileb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kkvjwryy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ojhwdacu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3axylbfur.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3muwjxkro.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3uzhmeaaf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3punjvrbu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qragbmta.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yudzvsca.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qilibbuf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3suzlmprk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3kvjvzzlz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3infeujsk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ovyglfyn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hruyiozi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rhndixpq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fmvfallv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eugqdgoo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dggwyeco.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3myqnoonx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qzuxanhn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jifdkugm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mehbydtz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3wuoxsmwn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3anjsyboc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3guzyplyb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pruwndae.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3khbaxlfw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ibtqbosk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3owimpaeh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bhyjvdug.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tbewzwfr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pcgdqflt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3chnwqqdt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fgzhgaat.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mrnlazyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lkhlklbn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sxyimpjw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rnbrcfiy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ygsvqffy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ghyvgjea.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pshpexml.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rzmadtxg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ajfggioj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dviliady.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3avuvkpdi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gwbglueq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lmkvptbj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dsdyhryy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uxiyhqcg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3sqiibcrp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rqjknnhm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nfwntvew.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lzfoiwrc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rxpiybwh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3clrubrws.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3egblcujm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsayqczg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ypgsdsuu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcaotthk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ekszclkq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jbvqphgu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kbcrcked.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ysixuamk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ynesxhgd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tkmwfbgl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cjdduyke.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gedtjvuw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xrhugrdf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3njjbxpyc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zkuhwucf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ufsjqxxb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hfmgzuqs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yqnjulma.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ewmnifpp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3lhatnrbf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rdwnnduc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3czllaanv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ajqiazeq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqlmatzf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfowirfb.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3krhgwzvw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pbibapko.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hgbzwdaa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iaptfuvu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkwlgvqc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sngutycg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3buvonkgm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipbekgnu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mpuvpbme.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pbrkhyvr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ctyshfsk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3twdlylqm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofsjsvnv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbqkpbjn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xumoqqgw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jutcvust.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vlmvkgyd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mteyiulc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3szvgcpxz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lvyvqefy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3duprvbbl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tjmqddtb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aqfrmxja.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nblxoywg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rdxoecwc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ptudrzgn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cfdblzlz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fxtsibmm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wpdbfjwf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zlrjpkua.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3abtuqlrj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cgvoboxi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ghwngbat.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3aogthtin.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cfffmhsh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ikiibzbs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ljvmsmyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lutvkjcb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pwbhodgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noxdkewx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ycwiatds.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lelsaqdo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kvblzazt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ecauhsyp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qdqiwtzw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zvyhtvsh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vryoayad.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sgenytpn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3eleqcoef.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bfoedhll.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rebrhcqo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hhtbieoc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lrpxtrmq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cjgbkksk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mtuooust.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yjjblowx.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ilyunpqd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mqhjkaol.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hltgjubf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3psxygpnu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3szxiirlf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wuuytbip.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xmzuyocw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pruiryzg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3bphooyve.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zpjxljvj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dplasgay.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ycaixkkb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bmzhtyoe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3xqqjvbhe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3twsnnadw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3daenvief.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hyptwana.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3oibhttaw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3msrjnmhz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gjesqokx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3trwslfmr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfslgttl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dgyoosrs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3oanrjqpx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jwqunvdv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kxmcuifn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tufeysht.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3abvszwtx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3spxhutqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3krnjrlyj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zhhhmjww.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vsokqngt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vivikdib.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ikkvnove.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3hcohzzjp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zyzihbdy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mntzjzjq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hkjkgrxd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3hopyrxeb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3wjpxknvv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3seslsmyr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xglrioac.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xiypbyfm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sifdmzdo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jhqadeyd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3viwrbgwo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nlqjbuvn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3viluzkyz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3htqgoyrw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3houlholm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nheopbjk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3upslvgzb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tvxdcode.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gxbxtgdl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3oxqtzxqp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zahwhlqc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tnfwkhjv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rgixksny.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zahyufhk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3fluqxjgi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3drxnttcv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3diqklxiy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tsuyrkoj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dqmdckxp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ihgxupgn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rnvaaidw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3atukqrxw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yzfpabct.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3glqxquzw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3naacuyuw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3outbcwie.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cegkfpkc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wpjmnghx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdwegaa.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lmwggxup.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ndwcwngb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vnlodeom.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wmsilwpf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ptgqfshq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aljucmhm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ouxnhbdt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3lqsabjjw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3qybgntpq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3litvugad.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3jwwhmeqe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwuiys.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jhfiratz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qmtqgnqr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xupknkfl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3rvnkhcub.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3gcrjbepn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cqrsjili.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kuqxhevz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jefwqaxc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3thkxgzdp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3udqhkhnu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rflrclxi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3inajhbmr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rhvghpxb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zvpypxlj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hmfqlcxl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wsrvlqde.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3gugalarb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tncscgwd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3agxfodpf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nwsusxwn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vpstfobw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3nfswkxor.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ldufhrwy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zsxzakav.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cxuhgkhc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mntyjejz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3wmgfdmqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dtllrdkh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3rqbfkwue.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jybccecq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3rhwkjpbr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3keekeewt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xpobjugn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eaxbtuno.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ztdecjet.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ronrdhul.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3urorahua.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3yxxwzhsw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nsmtxwhq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jminxxjt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zocvmfxk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qgwugfoz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vgghjmcm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ysrbqmsh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bwufuqjw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3cdlvvuwu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3znzggamw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3pspbscvd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3unfyubfy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hbfrssif.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dgtxdksb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gaqnfomb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3enfqyxeo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vtdydtnk.html


<!-- 参考信息 -->