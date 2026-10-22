代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2soctezfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kktdlpib.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gicwzcoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehzupbpy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqljhrlh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vyotukwn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ocmjnfqz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vustjtsg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pfnysnat.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mvtkpowd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ryyfnjen.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2srcckxyy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mvilbfpf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qyrkhsys.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sffesarb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2swwotdno.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mqhqqzqj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2asdoiora.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2upzjfkqn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tfplomla.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fxcknrmr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pdusxphq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qiwgrwkl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2cxgotbae.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dgnxsrvg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wkelpnow.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ardxzazy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gwpjoegz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2vvfmesbp.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slcvyfvz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ffexxgpz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kzqsxifz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vrobbgoz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gheodjvp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kzhwruge.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kkxsidbx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yjaqpaml.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2oxxgezvi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fgitzarv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ireyntjv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lqbcotfl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2upwtsfbg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oznrgfua.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ylrxdczt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ihkdqixf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bstgkuox.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2oafeyeyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gkgbdjzn.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ixisepnw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fqksslfi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2apnjnfnw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2olvuapon.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ybckwzbx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nrzloamg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2warpanmy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2awmkgdkn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2otcxfvye.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qvojmxmr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hkwvvxmu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ppremeop.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ltpsqnrr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2blpankle.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qcyhpbzu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lmdmruqb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkgbdlsx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vilpgcld.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rjuvwgga.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cnwodvzb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cefishbw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2woixurox.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lyippaou.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cpbpegim.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mxiwhfoy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngdpitql.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsqxufgz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2mmplawml.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nmqvbywm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xmidnjld.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2iomhzbmj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zwamoowu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kqglhlsa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2diktchxw.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ruhzyytt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kayrthwy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xmarxqio.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2clerwjfe.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nazakvrw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fkfkdfca.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oloohjok.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dxpvouni.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucmfrkqz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yybuhuas.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ahjdcffz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkudpeil.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ttpygryy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zmdlifid.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rcnebmrh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2vcjlqzph.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hakxnnwt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lbrylrnz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rtnsdhik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlffglkr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jxxkvjyr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wewmokxy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdmzfvrv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qsinauvx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2klhqtjqd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnxtqjwd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zkjehvbx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zesadcfj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2njpkfenp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ptlfjpam.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ukzbjvjk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kdakbnyo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gphngzky.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cvtnrgrq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mgjcvisx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fkihvtky.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jophodmj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tunfrlng.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2wiuvfugw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jttifyww.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2swhognou.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tdteirie.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ebsxmrxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyiaesxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tqpptkyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afbzhpkj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ipgbgjpi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fvpjweom.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bjjivuwx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2krwwkebi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ulopxolb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yjptwxjq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hnazespx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2aimkrygv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ivvifohr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wtulbxek.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nwzziero.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ycbnrkdf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ijlrndzd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2navxfyhk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jrbqnoje.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2iljnufvz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2kexrcmdv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqqahbr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ymechrdd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2iansqiwx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2esgksbhp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twgsxqff.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xecevtgv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ueenubii.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2povxeekm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2utdykekj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ucnkrile.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qnrnbmjw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2shuufpgf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jwesbaxh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2akhzezra.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2miaqwszk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2erfivsqr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kpwrmklk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mmjtfxee.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lhhaildl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xmldfolt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvdzwdvr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rajydmbq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fcyrefxh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2joeetsnd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xutnedfc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ltecixjo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xyfyjqqg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fttlwwxv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jhiczzce.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qcqxzvkk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2awgtwpvm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rzdatdez.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sptkscbm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2asacmwkp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2emeiplas.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cdovagcd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ukqordxq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qslolosy.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2fktbhswp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2askoqgcs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uzrjkiog.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2menjfryb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ozhrlukm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sotencym.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wlviqczv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2upjuwrvg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2gmhobrzn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxusti.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2bjrwxehp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sicsldcp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zwidolce.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zimkqtep.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2prvzjbrq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2scxszrof.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfqbehw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2qzkgeszp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2mqzuwnfm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ttqnpivu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2aeiwvqjs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fhnigspv.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rwcxwgyu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ufllsnro.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sdohhysc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ekmiiyeo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yqxagtit.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pavxsckg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2nxfrunmj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aygqbgmu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2xvibsygp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nzjepuzv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ettmfozv.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2oqawbkwh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cyilrjgi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2yjmkxdae.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ynplpifl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ainnjfqj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2djmmjpyj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bzrrbwmt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gudujogk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rmvfusfh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2yhpledgc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2oijetqbr.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bzxubimm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fuybxlam.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ctwzylgg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yklrdqus.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2srsfzxma.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ndlgvkbx.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qyxqkxps.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2wvnipigf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kooxaofh.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sxyysjtq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2agjlhbxi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rpxueqhu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcxjyvlz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qmtzmyil.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sctrseso.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qnscrxvg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lguyreqz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xhuomlub.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ogdclkcc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fmmmmdfa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fgidiisf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qtwdmbne.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nvjcquct.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kvcyvwvn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mqzvzerm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qcyjppry.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2srvgvavn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zzbrnphr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2juetxzky.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2iodeefwn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uwfihbqz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gevrychc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2mdusuxio.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kddqbkiv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gzlwdcyc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lcxonyvq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2xswsgkrc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fbmtxumq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ecxieano.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2oxhyplws.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2mbcxqebk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eiggxopv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2crurvwxy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2kxjjbomp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kttftkfy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kldeyaoq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2wrjlqsab.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bqrgxezt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qauqfuyq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rfjcixvl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gopremhk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2sgcjiraf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ydjexlki.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ekrjleaf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xtipptop.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ijtwuwit.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2cacpovjg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xpepcenc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wlwujddu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hcilzwzx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ayikhgoa.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbdqse.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ysjlsmym.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2oplcudlk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2izciqefp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mlgyagua.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ytlqzdxj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2tqijpsyt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ozxygktw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tqxlqjmj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2fdvnxyzq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2gdiuxrgv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2laiezooi.html


<!-- 参考信息 -->