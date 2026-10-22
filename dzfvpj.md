代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ejrhwvgr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tkmefjex.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lfexeqmw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2adyrdfbr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ekcvtzqo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hclpxbha.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2blzmeeln.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iclcnemb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jdqsvqrf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ykukzfwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tteheavv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2azgqjbpa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gxvvxehu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igfbebxi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jarvhued.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvcjygoe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcixqeqe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xwiramkz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2whffrndg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jvggrbfk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vzepemms.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bcquvzjg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2aevgwyoh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2oaljiyhg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jbvteibr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tgbpydog.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zerzahbe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vcqthorr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qlwypeve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqjygxhw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2biyxltji.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zjulyuqg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2irokrjqs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ytsbdxlk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2omnkkhoy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tjgzfujb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2shdqsfdg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tnavpaoc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ikpugvdk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wwjkaygd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sjugteyu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbijppmc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ygdubisk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2efnbkmvm.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zyyrykwm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vqhcmxpx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fdsnknxq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ewzsqswm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ditrzaod.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2sqhgwyum.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pdmtakzj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tdfqeetl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2uhlhluer.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gygennkf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yeciychy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2swoxrslx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yzqppncf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2piugnodk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xacudfnq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2flrlzxef.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzhoqpnp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2itcixoxx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kmvfjsvl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dwpxtkoz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oeiqxcsb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rcevetig.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uebpradd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vkczzvgv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jemxsovf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fpvchdqv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zkrjynff.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2npbkcvys.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lfzmwgot.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gcrmllbh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gahitifj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cugdaagq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jcnvedab.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hfqmjtnc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ulnjwktn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ushimlrq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gxbvwvvs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vaiuomup.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vaiwcsfx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2oqdowuhc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2btafztjm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogzccxsl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lglceolm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qoquzukh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tgourgqb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kqzsepsr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lemqogrz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ylxyvvxx.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rsszkskp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cvcehogt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cbhqmjcy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2buyrgzkh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bzihqftk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gbuxdheb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2evphchrn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uejwflel.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jnteamck.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ttmzpswt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ejsmtwsg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2whnsivyi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2skoirecc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cesmdtcx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2uqxlwbgs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfuounum.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lylfddlp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kbkcysag.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ktuigegc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rhryzxfy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgeytkpk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2naxwvjjc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ebqbisxb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mnacnojs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhuujkq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxixzyou.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2snxvrhrq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ilzllopk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2whaqkvoc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eyevivhc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cibrsydg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yerzrsiw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxopdjmg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2chnrbycz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2msxqmxhl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2igcchqjr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2scbcqtox.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tpwghoba.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdledrm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2crbngmed.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pjhyuccs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vixrtbqt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dtuitkqe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ykhapdng.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mptqkscq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpfnicgm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2letxzzqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbqxowdd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qbzqmjcm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2agoymqui.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ndoaovjt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pobxsrbw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ygfngvji.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2datfoaar.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rndwfxts.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uijhdgtk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gxpndncc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zjnnfyhb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wkixjszm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bcruubdu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ogxncwgq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2cxqiakrs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ohxehpxf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qoquddap.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sloolbsg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2irgwwqym.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gzhekqks.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2oaguqyvp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bmotrfmu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dnennhlr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2myufqpkd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tapertei.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjqoewyn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lweuqkrh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bovnojfo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pinpgefe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2njsomxxp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cxiuggmr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xfujqxgd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xerrtviu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2gqkcpbth.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2viuwauyk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2yireevwc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzhmkrr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zuaodwwn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2kejxmmgm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yddqmnfg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uigplisg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mmjfgjay.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jyqxmmwn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hlyhupga.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tsyefjux.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2crmrvwwu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wnqldebe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iikpkdxx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fihgypoc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yxcyaiyh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2todwplgz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jhemtgiz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yiydszwv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cwefafmf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vcqsqzwe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zblbnked.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gaxchstl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2oahnlrbo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2oydtzopo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wjndrwgc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzhosaa.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2xtxvwebq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2dvmqgxvl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cxpmtszb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fmnyzztq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dwhqnjwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xoxpeumj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vwimljik.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2itihzlfx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dodbcomr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xhnyyzlc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vshidaav.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qzscrdvz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dcbyaojq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2qrrajitp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sycxoujf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uhtcifzd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pbwddqvr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2mjrkcjpp.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2krqhbfam.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqovbzmg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cknhteoe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2aygogszv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2rwwuxjpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ntkwuffe.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xmavdakg.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2niowrqfo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ngfoamwn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2btruuedi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zywjiyov.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blbxiqpg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2booyqhdc.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2evkasold.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnltudob.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wbjvuwsq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qyabvlpq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mgdnyals.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hbcnnuyv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kmjsztor.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ulwiqewi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2hxnbmzdd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ossmjtgh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2hvutyyut.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hplxwxdx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jxhrgsxh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xdqafqrw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2alkvtcey.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gkwipyfs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2thhsnjus.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gxlewbmg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wspjjfkc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qllfwjca.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hrxkfqfq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bosgmcip.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ztdnqaxy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fqdsfuyq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lhfdamxu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mwmovwem.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2abkzianw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ttndxnjt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vncalilv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wdskuabt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oqmurohr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2tvdjimsp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ckainzph.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hyitemvh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dliqbgep.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2wnpjvlzl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2rsspzygt.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2lpwhjacp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmntcajr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ydirtmul.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ilmqgcfw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gjkipebp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kzzxhaae.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2xskgiduc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xvwotuha.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2nndtqcgd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2izljbaoj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gozkxbmg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2goeeqcff.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2acyiojdy.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2vaohxrxi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kqgbcumb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rwdtoaag.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2umnbooqt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ivmoqopq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wshhaope.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2yrsuzhnv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2widsvljh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ujxuzluv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eazlfxrm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2jzwikhbe.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ptlsjlov.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hikqaemf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eyvjuxrr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mgiszozm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2qwpgrlzj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ajuswmkr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vbkgbnpf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2dbubgxfg.html


<!-- 参考信息 -->