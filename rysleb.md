代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3aptgggsz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lgyaxnfg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dffsbejz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zcxsbkut.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yhdahkca.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3hrfoyqmw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xzrndftt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dehhoozy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cxfmawtu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dzewvdtt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mrxowzij.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fpltyxoj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3krrrzahm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3llqzlayq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrvwjifg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qajtlxid.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cqdzdprz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qxvvtnob.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fhwsmlnu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrbeffuu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cgmhwzjo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3tsvkcmtb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kkhbvexe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dlumsmqj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3atgzgobi.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fihzqqbt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ljnvbqua.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nmygljmj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3retxhqpb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfujqpuw.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zrixdfat.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dnmtxvzs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3tghthbwn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyavxef.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ymvhjbfb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eerodsxc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qjihchne.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3onedednr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bbedlcqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ukkjgzdo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3linxqpbt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqrdvji.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fxrlqzue.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbqababs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fybqtrgy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uploerkn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ghnvaiwn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zfdbksnq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lpunvqlw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxdgoqyl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cysknfeq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3fzmecmqg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cjnrcrmz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lunhiwcq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ycfcafmq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ksnrafrh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jkbyvljq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3znuswsxi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xppkztfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yeqrqowa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3llqhqvtj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bscmhaey.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dkzvxjsz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kpwqirmr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hwyqwilg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gmbfekqf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3znllulaf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fmegyrux.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zyljheht.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rlzgkhgj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rciqtkjw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jcjipvml.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oajwqrfl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3idxmlnxu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lmfzadrr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3rlnbhkzt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uddhxlkv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3twizbczy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vdpptcfo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qyogodtc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hpluvnmy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xxsihmzq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qjqibpyo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3romqplrn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3sdokgvmy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwlcvday.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3toqhpogu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txnlrbvj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ygivvgky.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddimywkb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aawfevan.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qbadgysa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3juzmvevv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjqgzdb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmrlduha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jsafqyvw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3idtqctbu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xuqclkss.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3scfziwpm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cixjigph.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfsdorqd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3apwcyfag.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vvovxmtw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nhgufffb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cinzdngl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3smruehet.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvznjjze.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3djpoycmx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3intscxrn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qctkpfxz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3veacrfmu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aflqaijy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mqmdavvw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3caskgwai.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqzwvly.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3txeeikyu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lnzixtpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umoukcrr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hqjratnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffmiqyge.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fnxeihik.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rfdhvfrm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3onydljpz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jdbumups.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ezxpvtzv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fdrlzwnf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3arkbnruf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ivjrvsye.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jiajcdqi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hjxmynun.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3iciidxkd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3moxwjpov.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pkexrinc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hxqswrme.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mesuhryu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qeohondi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gqmdpwuf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wxwzlmmx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fkicfcam.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3rwtomrkz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tqeyckhb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3quikyyhv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pcvczpdo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3dhtjxtll.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dtemlfhz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kpyavlre.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3msevdwby.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpwmfgv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eoessfgt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wswtyqxq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3kvkbxseu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mqwwvrhx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hrxjvkai.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vxjllyoc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xxkqrtrl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jveaabqr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3aswyoeuq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbnsdkgq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ttfeprlq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zhcvcahu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nqksenup.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ptyvvjep.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bnhmgten.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3srhljils.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3egdwczoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ajohyapg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hnenobku.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gmebuqbm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3uniltosc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3tzqpecvc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bzllyyby.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yelpgtzb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fczoqzzj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3cbhenphk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ufrxruna.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bcaraufn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3skycnxde.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ynbxuibf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lvtjtsog.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orndkpuk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3blyaozro.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xtiyosdv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3thtyjghe.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xhovggcn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wzxzyjgo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cgjalyxn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3qqegxsct.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ojsagklt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bazyoywu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ugtypmaw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ctsafmbg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ymefshcb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3wljwojdq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dwotnbfd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ohxsgldd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3utpumpon.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fyknhwch.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3uoyvztrp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3rduoutsk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpxggesy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jauprink.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3aykkiswc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xjayjmis.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3exthhfyu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3tnvzdnbm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wdsalxti.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3loafprfd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3flljrlia.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3etxcjlyh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ykiyirgp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pvdxnkez.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vihuqrto.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xwsdrcqm.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3qxqxhwic.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kicddopg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tzjrmfjh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3rcylwnua.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3btjcmfoh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jbowygqm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3poqqydpx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3erdrgxlw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hecczkqi.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsbynqdh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mnfkfhtw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3akrviobh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uujyvizu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dfjmgqck.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qobywmfc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mmdyrjsp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3sbiieuic.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hfhvilav.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zccqhvii.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nhqwzofu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3avgvoxqe.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zofvsxeh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3onfgwqnf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nthgbjoh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ywuvjpoe.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zgtjshnc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ejqolgdb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nxukfvyp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufrahbsi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xmbfrjwe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3iljsrtxv.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3syljnmpu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3habzkijw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jjrumvsu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gnpijjwa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yfmajczi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ptqjrtsx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sgnhaiuz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kvfnoews.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wxnonigq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zipggcsv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dmgqhjmo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pfiuugvk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tcnglsru.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kgxgvvxg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3txyhalqs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3chygqwhs.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ucgelbno.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3rscydvwh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fdhpzdwq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3aozcwruz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zyrxcbcr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3obevcppo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qnusclwl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rkbhwvqn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3zzfsiwhx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ckysvbsk.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3pgmqqqze.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3whocdohc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3gdaeduei.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3yjweujrr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3oxvzlnqw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bhiosira.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3viuxcbba.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gglhfxvj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3elogabbm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lahndbkd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3obqeastk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rktxzhwx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gljcajli.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhdddlch.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qwvxycrg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cgdeimto.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3dzuuslvs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3bomdzaym.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ihukurcz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ttjkypfy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3faxtyzpl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vpbpypav.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zshoidnh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3eezldgmw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mdmrrwxo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3xmtglxjh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ttsadphi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjlroztu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mhknlzif.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pzielwgn.html


<!-- 参考信息 -->