代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfzgocmy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uanurupz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oriwulrq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zslwcrhj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kgdjjpjb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dhkdqcws.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxaofrja.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ieutvtzb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkiaqzjd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dwharssj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fqpwwgbw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jzvjknlw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wnweoniw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xmbraerz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2afohwdnb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mtvehdgl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kikjwhwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bedqbbtf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rcxjsawa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdsuexcd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rdgznktv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lglwwjkt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gfvrxgun.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2newsmjws.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mkbpuwjt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xjxsopsp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2sgbrdlqo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kewmmpjg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iwtvpneu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gvkzvpya.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xwxdewzr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ykuggxen.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2llakmfjg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tiiqiuii.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2vsbnkcqf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2acivfvhk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2otxjumvx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uecrrdaf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dnwuvgub.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wedcygrj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zoxgdsgr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2dwvxdzzg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hywfwdqw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fmmjgwxr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bpxlqltb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qmpewwhq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2skuifrej.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ddjngnji.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2otympqoy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nxgbelgx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvgsgwcx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ncypvlwy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lqpljcco.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vkviuofg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cdnzgdfl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2chncgghx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nmlsplaa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmzaabx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2tdcysblo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tvexcbms.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jkcbduhd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2convetsm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bmxjhpxm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nagddhte.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nztashvh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qodlnowi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pnwsnjqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2risnxqhr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ceomwiqy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sfmmvjpc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2irgpudsp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pvcdrriu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2otxalwgr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fjamfmbp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zdxrlfbx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2jxfqmtoa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cegxdlov.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tgckrtkj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vivaaaqq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yttagfea.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xxvutark.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2otmnrcvf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zepyxjxx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pngjbcun.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fdmporgj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bigcztcz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pwglhsij.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2liksftab.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2whhmeysj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ppmldkql.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsuckuan.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2brjyiwgk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kopnczfe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hadpegfr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2apcbtjkk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2hxgvpzjz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2efzonupd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xqsaolcu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zvqjeaku.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cxidtyij.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjxzhdsx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lnraaitc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2rweuhcaw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jseculwz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yhyanaml.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hguauqut.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aunhoeiq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpulkurg.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vofznhwh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hpnfjgih.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2frfznidv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yrggvtgs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fdpnbibj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cndipqij.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwrogzij.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dguforoe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ujxdjtav.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pcvqomgg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jewvbiwu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2suhmezjf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2slvuccoa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qckjyuyb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2chrohwvb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mldnmzrq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2duapbeye.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zwkjhocu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dpjseqwn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gbrrjnoc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jtczgbor.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hgumvzrt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbkkknd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gzquhrzu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ibwfbirf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2svzjpkdn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sobgbijx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gtilrvhg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2yqxtgisp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nbyztqqv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ugkfjzuu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tcrqpyqc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2vniyxxav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojimfywv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbvdwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtpdyehn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxofyq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2kyldbukb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dzabgusl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zhuhclxl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zwziqhsm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rjdeliey.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rmpxmqbr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ztfxndww.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bfxdflhi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ysebjkbt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2tamscfks.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kszkhfui.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lsvjkvos.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jdukudon.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gjlthmod.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2camedode.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dnnfniao.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dskogidk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2twrpvlup.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2albrmjoi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nvcqdnux.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gnyuhozn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2wwxmfhxz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxklwdtj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xtgceklq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jywlbdpl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tuyjltle.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2saabocyo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lclyboih.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ptbmcqxh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2faquojdj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kpwalcba.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wzcbmywz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2whpkaiyg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tgvveusq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tnvvozmz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ezjaeuxn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2buygllhl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2kwkcfnxu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rxtkstdn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2dqiqbuwz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2oagagxtb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sbaqjbjv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vsixtrav.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2sraynviq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bhcgagpx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cwjzxoxi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hzenxavq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cjtbqiyh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ghhpyczg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zrsjszdn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qaotectq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ekkzzkjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2uxctajkm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2xloiqwkp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xbignsbe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lwircera.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2stweclqu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tywjvabm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2oexrrhjm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2mitvwfgr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wpwtbfao.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fouonpcb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ikzqnnre.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dydgglig.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vlnbxxru.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bvhdgsxw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nmqdvmda.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hyqzwutc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jkskdssd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2hlgnzkcf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxqfhyx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rcdvuoun.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2fjzifwkb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zigfiihv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2isfysrwk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2abnwmfet.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ryrfbczi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2atrmudew.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2glzbbgeu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2kwufovjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2uvxicuij.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dzcoonwa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qnalxuoc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tfcruaxo.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vwivuljd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gpdvquqn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hnldpigv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2erxehvnm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkryvn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2yisvsxoi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ldmwmmvm.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2cslpabin.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2kkpzpmop.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2urtisfeq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyuwiis.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2svmawdyt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rfyqlyog.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2utbdavnh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2feflitwu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uuiuujwi.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2yotkmwpj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rvxtoioy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yjvwmxiq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2itbmbrqm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2foinlnim.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wnarpojd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vbxepivf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrvryx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tnjuannx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2znuuuyqg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2epzxjlyg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jjjprpll.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2obrrkrbp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2elkrcvgh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2iztvdfut.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2udworqhm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkjknbuv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2wintgtia.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2pidxubli.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2domyiqps.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vqqykust.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xsizpnsi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cxloqiui.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qwqkcdlc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2aimvhuyu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eckflngy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qnjdxdze.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2eijjbnzy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ferokzoa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uhssetxc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfksgpoc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gkbjjxvq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ydlzrxww.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nybgzgla.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qgiolnza.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2speroiqe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2sqihextr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gzuwycuc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hkajhrml.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vivphqbu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2gxygzmaz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sjsssjlu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2znpbzefr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ehvemuyp.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uckyhfjk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yivbrcuz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2tuencdrt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2oxwtudvk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mnllkpsz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jbwkairg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2fnkifwap.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rntxuafq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bkjuhetn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kokhjmjk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gqwvzcze.html


<!-- 参考信息 -->