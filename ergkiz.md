代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pvrlxrxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upqldyaa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ggxcjfpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvmtcsxh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqlopumz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lzylkidv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qejjiuad.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2otgmlbie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2adzhuavi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gqfqurvz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zrfyjlkp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ywgqryqr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fufopcdj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tsqcycbx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pkwzwnby.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tubvdaku.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qwnmosnv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hthdecfi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mlsctrzg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2terglhiy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bxqrojjy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bddwllxx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2sgvyosrz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qdxxpfax.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qnwnimvi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2sygxsdeh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xutoykqk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2csecpfxj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ojyhbjlr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2satqofvy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvsfpglo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lcvylrxc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dfcrdplx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2phtolmbz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cnvpuoyp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ygpdxlqw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mvbriwlh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ozrdvtux.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jdmluswm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ipxgyhlt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ipnksufr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxeilgx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ohfqogge.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmwjymh.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xlylbzxl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttznejed.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zrzqwbxe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lmggfnen.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqmtmfob.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnktuax.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2oioniugt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hclufxxz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nlyfpoec.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yogsxcmf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jfxnxkrx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nqaazszn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lcplpqqn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tbgnlcif.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ibylofnn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zhhwobsz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nlfnuptr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2oczzgehf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2wdfjjqbo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iyrrwvpr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2knoakvdq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xdpsmcag.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kspcdqdr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ecvxfudf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dvxyqodj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2oqsatakx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2kjkttbya.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dykpdijk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lwvckttz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fuuakgjl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ykrtzqwy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ylyfgxwf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vmdabzfd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2dkflmnds.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fawtiniu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cwzhwkdv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqnouovs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jucekuve.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ljnpqxnq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2iuutfmah.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mktankvn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aylpckmz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tyeumenw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2iidbpits.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2suthabrv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yjqcgqfj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2abyuaueh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kwnfznvf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gqxiupii.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kfnwovtd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yefnjosk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnguqvkr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oxzyyjba.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdidqer.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdyepuut.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmqybi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzympood.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcecdaie.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2naocmpwc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tojdobsa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvawddh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oslrcfev.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2foaygray.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2thaooqev.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzcmilpg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kkgfdtjk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oxmfnrzp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bhxsjdqs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xoqhlcfu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kezwuvix.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lerbkmgd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ndnpijdu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wduiimyh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kglpumkd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bgquuiyl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xlwygeab.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xppyprau.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bcyhwjqk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqclehq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ekzodhgl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2azyarwkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljgtoksx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2raygyvdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tngjdgbp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2okhbwdkg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qyvqfpax.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lkqvigbn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nzgrgrak.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dqzrexqx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fsduwnbx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mqxdndvf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2taxmzwcn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uybbbuef.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eygsmork.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2uwdbakja.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2oaqjcrap.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zkfchvdt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dfogvpiq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tmmthnjf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2oqhjvrza.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2dcvyhzkb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2djyjwmrh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2kiqeccjy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2bxbuvyql.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2bzteahcf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2geaojotz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2uebehoyy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vkhcyioi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mddvbjam.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2flaxawwn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vqszwosz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhiiswd.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qncbpbzc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2eoqpiqex.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2eqpdawfg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rwwibgst.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vdmqvefr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2nujdxabs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2zallgtnr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ecxsdfcx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lllzsjix.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wscgwbig.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wgnluxhb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtleczd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kprouqql.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2tyuztgkg.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2lroonhyd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2crpazuwg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2riozealm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wayxkwkf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iocncwip.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cxfhbscu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2iaywdwfd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xutxyndb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bxtprlhz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuvmrcz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vraemrox.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2vtpdjdes.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lpdpdrff.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ruowsvld.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jgvcqhic.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2knzxdval.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fmmoxgmo.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2jjgdckgw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nutphpqc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kmmvkcvj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2reibcdep.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cqiuxcjn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jqgehuxq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2brwvoiml.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nkrbemot.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2shiovbnf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2fmptpbwo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2akhscvkk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zzjzfzpc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmomiro.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xbweryck.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2nmnaswwy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ysqbrfki.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2thhbglzg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2vyhdfgri.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rrzcmovb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2zwwbtavf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gygxqksm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hvcvwqpw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bjcixewu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2amvjkbnc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2frjccexz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bxfqsmps.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ljlhwqfj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2etzhsxuo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzsxipw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2eoelcryh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfpjeyx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2atriqnoj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2bstbzjjt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dnbbffln.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2iqmzgrkg.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vcwypyfb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2izdhduoj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2dqgexmnr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2avnzrzci.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qrlaxhki.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjkkebrx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kgdjgnqi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gfslntub.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2awxllkqu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ipavrqjj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ewwjzjvg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cjgeuinm.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2fywbkinv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jhnwpngf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ogkdoarx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ovdeluwi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxktxcmr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ismffeds.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xfqmcfor.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nsoskthz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qdybwbqr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mfqiqfrw.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2fubggnti.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xmhapcvf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gfehmywr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rngsbnbz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mcsfpvyy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zqwkykbh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2vnzectui.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wkptjmky.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2sxvipyvl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tgmdinde.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dwwhqzlw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2tnunfwrv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2hkrimqhg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nxmgeizu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zgyhlrqc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsewxjyd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cqudfpou.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dxbezlvb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2nocvsoro.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2whnxebjp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tivahfdd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbcplwva.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gyfytrii.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2xffjlfgh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ptxerslv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bccckdpa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sgjdifnt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2gvyfjydl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zntvobho.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2unmthhgx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcxzrzrf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vcqaazge.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2akgaynzd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ktbeckta.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2esbuykls.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2cwvduxaz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xoqungls.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2koizwsnp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lphjshtw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jwrzjfzn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rpqqhpmv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fpgbwpga.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fjtdkkii.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2wbzatzww.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2oplmqyjk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2kagontmw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2iifeewqb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vkekuwpl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jabjsnzi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vuiqwqzh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2azgxtgqb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2klybrjxo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2scisvcfg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sihybdkl.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zegirafa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2dojyqfhy.html


<!-- 参考信息 -->