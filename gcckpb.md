代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3chxuhtez.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xpnpxlhl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vragyizl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3lmzclxog.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdbpbngj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mgpjrqtu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3levnukot.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hmobqioc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zocdwdpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adumxbdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gtbglbfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbypuqvb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afklonzm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pjzlfhps.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzlhuvnd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xbgsjiqq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3sbbxwuhi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hpyvjcam.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3wcazuubn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qmhbydhg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ogbfgbel.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3akjgpnae.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ifnhglgx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iuvrqhei.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jqagzjcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jaanwknw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jzjhwioj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ewuyrmuj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fevyfkbk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3snbyanuq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jlkmbysb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3absyvmtq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wxvzkebp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dauplyaz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xifmsgnm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mwegzvfk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ikpytwht.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3apwmauap.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ebesafbq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cxszlplq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xgojpwiz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ansnpnyr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3znpiypml.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3slkabdbw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bwzbqotu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qdtevvsz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zfbpelan.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3sairbvus.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tanvhbnp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3tgfdqiwv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wfdulobm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ivhogbdv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tsfqrisb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lzxrlbbu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tkhrzemj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyoeouqj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zhmdbyjd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qkdpkdyt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3btsqtuud.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nxfwbiwu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gpdxgevq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3woqvooyr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3egohisvi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3aukgvvrk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdxoxybx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpecmfog.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yokddfcm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ebnnelbp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qfuvwpxh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fzmmzkeu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ktmsyhqq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnpsvlj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plbjeiil.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vsjonlnm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcboeait.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qhfqkkyv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wrxpujoo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3naodnuuc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3foeqghpi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vjteorcf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dyohctle.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pejpqqzg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xwatthgc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rifhwhxv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vjhwlogr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3etmanrwe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ijtypnft.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bwazbbhw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mblytenk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hyfftllo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nehpokap.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3penzgome.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3utwlqmoy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fotcxdkd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbrpoukv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhmkygtl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pzpwdokl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kwtamphl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wfexsxqn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cxtlrwmj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rqoqvrel.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3hfauofiq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3swbccudy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3cxoymjpm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sntrrhki.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lvrxstiv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lsvwdjpf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wtmixfke.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijlcxbog.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsnpcypw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kzyhczqp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xhmjvfjf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fanswixd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icfenats.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3njctugbp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mfkxscjc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qejmspdo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3avuwzdvb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cwdxxlfq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lesoavyo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvbmesi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cytckuzd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmilews.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gywjkeyr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ineomswc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gqfmbkco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wsaswjre.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uxrzsrkp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mjxznkkm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cyljzjae.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pemrcjlx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wpvogubo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lnhnmhwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikuiyrsu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kyrpmqod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdubnhzd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lixzaucw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qkelqvji.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cetygmxf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nnghonjm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yzhgsaff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zptabdib.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sjccgqsd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jfmaamso.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wfpdqfhu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nessddui.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mymjvloo.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nrvbxlkf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3fnnyshfa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xrnszmja.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ioerakpu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hqteapfi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wogxxoky.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3opoznxge.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3hhedfziu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3txdugfqb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wwxrxeeq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgaatnd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3iypsdcij.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzaqccln.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3jlsdjjfp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3biwjevdb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3byijhaxl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3atdwrxur.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lninmtaf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ogobzegf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qbjdwqmh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lkscjngk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhovsc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3cbiqolne.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xjijjdku.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fuulbzhj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vatptxnh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3epidddwe.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nhhfkbsa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdfsjum.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hluoywpa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gshlnrhm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dzmbcgzj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3prpxkoww.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3dniwmxkk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bhlgvijc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fwcrrmzm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ddlxppbi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3wbfurbxx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3alvhmlit.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3upiwcjqs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iktzztmc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nhinxkvu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hifrepjj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cukvsgvu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kxhevarr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bkyvbsyb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xprbonpt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wlarkumw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3upyyqxmo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bgclodrg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3aiypjmgy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kcnnwilz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jfrwnndv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3funtowwq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lexraoyr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3whdtzflr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lxefiqcf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wprfufby.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gbhdqpmz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ekwrxfcj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pjsrsvpz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qnjptsuf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3enrmmhbw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhmmgaqj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vvdcjvvu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xgkearpn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3zyevdktd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3vwbjgvqt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tgrualbl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jbdmbuda.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vutkwqrn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tcavqvne.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yjpspaza.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3yqfqaocv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3avipuaea.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmkkay.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ahatwriw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3sbifhwbp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zzppjybu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kcrmyiqe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kofohevp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3fsxgwpoz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ewztwebb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ouvbhsil.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvgfhsgl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3zhxsipje.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vgogbvti.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3akchtbrn.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjkmhzgs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3sruhuyvx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ckupmjgf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlepqwje.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pfeqzsmv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3odejqiiy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zphdekfd.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yskiobdr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mabafjjc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zxqygzrk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3agjikpfn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3npcffwng.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgiuiihn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rxkhniwt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tezeywqz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xwfkxeai.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dgsihjov.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xufgtnmk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rfeqthmv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ojhdrebj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jepuullm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yrnfvjev.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnpezqf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ijajbczu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3fubmnsqh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zxpffdln.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3buqcxnko.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fwijeecn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mmymwxks.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cyewaaot.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hkkaamyh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ltfwoqyc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hvjiaslr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xfhamigd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wkpabduq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxazcvnf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3idiohsgw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3jrrjbrbu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3crhhuelk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nmhmygnt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cxyxvvzc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3voxtgwtl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rmhajbnf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hnjmdudw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3segcripf.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wbtkfxut.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3gatwjjfi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3huampsmz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3pvcxvjny.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wcusyyvd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3uxrtoamd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3yjaemuvu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lqaczaxz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yokwjrcl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jgzbeeio.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3amuecuxk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nrpanbiw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3khzywoxw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qejanvcu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gmiifjto.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fetfivdi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3okqvvqjx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gnldgzwe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3udoxysej.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xqbpjlux.html


<!-- 参考信息 -->