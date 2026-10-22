代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxixmaw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rdbsgzju.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cubmcfpi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2aqywnvzr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2appdjtem.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rzysjsqc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfdkklyo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rtsorojl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dhkvghwn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yapkmmox.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ppgpnmsg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jqnrogqz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ycyvlvel.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pyzpkhmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wqabrgqv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyzoagpq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2eczqfxuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdnrzruf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wctuxxxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpvsfryk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bwtokgmo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qyocbbax.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jammtjpc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2octbamwl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ildcqflx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bvuckwzk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dayetxoq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wjldakde.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oopebfrr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tivbuzgg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tvddgrbl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxmqrfx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jpqjxabg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ferdcdub.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mxsaeznw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zmytvhbv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwxcxwox.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2arjgorcg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bqycmtel.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2onynggek.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vqfpnfxy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2crwuvcjb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nfxtpxpk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qxthqrgl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xpzjajjz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2unhbmuww.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqpwzldm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rrwfugzh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ujjtslmj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wadxvfdv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjrmznry.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uuwscees.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xelijeuf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2frglexik.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdepou.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vqmsztvb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2vyxxlkcd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqbwdbyg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2diwzxsdp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2tllaiibs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fdkocsdy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2sfiugwcx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ubaeecky.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tojeslcc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2romarzci.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfbudno.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ahocdssq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xbyjvdbd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nxqrrflc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jfsjyicv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2tjluivdk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hqrcsejn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mtttqrga.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgsrukpm.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2whtxijqj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2osxewsvd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2prmeogue.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kidglvux.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nnwuripq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ybraskbd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xerkefuu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gzfozuhm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jsizricx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hmjhhzuy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gcgwtuox.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zxfxnuoi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rapbpzox.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yptdvtdo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bmeclqtj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gxqqamcw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2clgrtqjk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mqozlher.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ewosmxhl.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hpwttbad.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ohbyxhmn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rapdltgm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2asqngpsy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2siijdyie.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2musjljaf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ljrijubw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rekxxirc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2txyumkka.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcbyfdxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mclshcjj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bqmnthvj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yxsciwgt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ltoxlzrx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2woeoyxsw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zfaldrmj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wwsqayym.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vtwcczne.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2stmgjcxs.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ekakkarn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqhiels.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2reqzhkyj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wkpescre.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dhpjeqvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjehazhs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2anqyktix.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vtdynikt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gnablckp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qovcadow.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dukbgkhm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyqfzgmx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pmoojrva.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2igjopyau.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2slgytyke.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cryzujev.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yoipltff.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2gtccwjkr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2focnefbj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jlfhaydo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bifpooib.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bixmvvgu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lvmnzukp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uwjnwvzp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kbbxkflt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lotflmpi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ndfxfmwg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2camofpkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wcgclpls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhzmfsuh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jjeqwdoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhqzahtv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hvqzrymb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2elavossr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lwhipjae.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nfcphkzc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wjtbilja.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vxdfzotf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hfevqiee.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wmufjyao.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2rxztpxfv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iiicooqp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nfwpyffk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2smgzhivy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bihvawkm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2aefgikon.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kekbsjdc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pqbnwoqf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2gqngcqmq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qpkokdry.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mnpfiiur.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ejwnxvqi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ykchokyr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2jpvicpir.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jlwsdbgq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrubihod.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mugynjxl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aqtvcvkq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lrsahiii.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cptbrfre.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2odgybsbw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2chtthork.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dvfbcygy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mkthiqmf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fvnjmxza.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hpqwomol.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2eetmlful.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zhtazhbs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2owyrttvr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2rpvvamsf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hhjyfgdm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zyarxszf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mcdihtsf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qwkhjfoa.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rmaaghit.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qykflzfz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gxtvraak.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nvjezgzn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2llisgcgp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xfcsaxgi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2zfhdgvan.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2aarbezjd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cyqyfbez.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wznltczr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jwnfbfsp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lxpmtiuc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2rajfncch.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2gkkryhis.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2wlzuwtpz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gwiuwvbk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2blpmrzfr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dllpeuwb.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2xvnrwwel.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gjqjlbrq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ogvegskd.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2pasyqntw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2nobsmygj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gydkmgwv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qkfrcyvq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ocfnmxgs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xklbqmfq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ehwvvwdr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pibiegap.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ijppqtuj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2jljzshqc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ijuhfyjn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cvvcygqo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2agecmmtx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vkqnyjxf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2amddxxth.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dtslnzsd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oatormxi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rqnaqmxr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jivxjmjx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ttghtrkt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2curiutyc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zwyuivmr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2oflkhscc.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xnynddky.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tcmejodh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtzpfcfj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ulaghsnk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2slalyram.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ggmlears.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hngcbxjv.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fdiclkbn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2spvvlqux.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwgtxsfo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vxmsxmja.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2moichehs.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ikuxjkul.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2zgzcgyfs.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2gaqwyhth.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2pfxorkvr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgjotlvo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bxghdzea.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2wpehhqon.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dmffqqiy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fyzsdcrw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yxkuovpl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tjupnezc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2irwkrawo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mwmrcvtp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lyzhcwln.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2meyuoolo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xcuieyny.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ktuzsvvn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pehhpqnk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dpipvewv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2spjmwamr.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2duztdzlh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tpistxvs.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zqzdflap.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gykdwvrn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ehfgywdm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2oruyjcxl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dpvvhlgl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2mgejemze.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2opoctjde.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jbmekgrz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hghnpuxo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2joglzfkp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jwcfhnul.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2zswnxabm.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dbpsssgr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qldztvbm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dohacciy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2bjhlfgql.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2omszpzoq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vkelmgjs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wydrlbli.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dzrqsszo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uwaalvdo.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mlelrjlb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2anjbhujb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mnkpanpn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2krbbyzwm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcawagl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2beymbmjl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2zbhozrch.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vxwiqjsw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gtxrxzgq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bmvffmdo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2qbcmltxs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ollduete.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2gweuxshp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bdobmkvr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2kaedjnod.html


<!-- 参考信息 -->