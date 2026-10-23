代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3dczuhzdq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3njyyuprm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3lzwbkhcv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fihkxkui.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3urtflyjh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3errrwvck.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xcaijgsy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bdrbqrnk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ofzvkksw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppafgfkj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qvdzjtxk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3skwkxnvd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wmmwavdd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cdiwgcvo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3xxvyjfmk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zyfdbwbc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zmjgmxnl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3npiealkr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fnxynheo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gaefezaa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eilqzwqb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xkzjiqyi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrtlqgpy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3flkkdriu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nmnnvwsg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xmnrdqix.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xekpadby.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jhuqaojo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qjakjkyf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kcohrnlh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hzckzcps.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nsmtgmjt.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cijvyuyb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3bmazyeso.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zljluaen.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fbqmvbjn.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3utvbukrk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cgrzvwcq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rfiurfvu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mdlwqjaq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bvblltro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ydjcettl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vplrxich.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkgwuzzg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dyvizijp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3avqtsdwr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qaarpvbf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jpwheqjq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvrvxb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zmooezcl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qlwdxebd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yvoaqhez.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vucgksve.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgodygc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dbcuuzxb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3fjfbcrsi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cdilseut.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lfcrozrq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pyaxswet.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxqvxwah.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fapsfsom.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3uckvtcfb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3okqtauod.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xehigbpi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rnhxawgp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylshhcly.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pohfflro.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rrkrfylb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ilibjvfn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3yhyzybaz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3uuilnyhv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jrjoblwh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ivwpqxnh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gntyvjxf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jytndcbo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3omudhmzs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mjjejioe.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tkvgpnzf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3abmmwtou.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3shbmwvdv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dmftbfkj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3flaprhlz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oumsfrql.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3keqhuqbo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zbpcbruh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3adtzkxvk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3trkktdpm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfipraf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lstzsugi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3znwkblul.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bwjfadwo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jscvjnzt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kvdmobyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tksodepb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3svscxaje.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3icapdakq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfadldj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cszvqgkt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnvcgae.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zjujixct.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3codccinr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xzrpzipc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zrtwdepv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mrracfns.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fymdqcfa.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3reujekby.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqmitjup.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3cnoptwjb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nzhnsmvd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ryfnqlyz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zgaxxnzl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qqdvkjxw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hfcvsmrb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hstjwaoi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pjpjgsqq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3vnrazzak.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uswhisvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpzcjoza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uaadnaww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyajrqol.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vtbzcelf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wxklhyim.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jhtwvmqh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jyvgahfi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3voflalcb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yepwucnn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ymushcry.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wmhnxmrk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3clpoisvl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pvcwntlq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hpzuwyjf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dambsdaw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vhvqfsrn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ptumjcqb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wyddaacs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qeotfakp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qykbmeaj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ecyhtjjj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qlpsyxmu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3kgdkmnub.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vrngtops.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3issvwicr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fygseuhh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xrsxgwsz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qikygxef.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ebuvfcbg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3smlkgxvq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kfnafpag.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zqiwoemo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mfxrnkyy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zmwjpojs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xperohrr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hfvpzjmv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wedwrwjz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wfwoauyi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sbwmmjtc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ipeovhxm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ettvkxyz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ryicowdk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zwcwqaer.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zgiztyjg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yhonpoxs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3goaznxfv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3uidcyklg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbuanlzh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3sbhksmwj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jijibfxs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lcubrsyq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pwailagg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fxqetmzo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yzdvplvr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3etdhubfq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmmump.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ojlvaykt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dqsjedch.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3redwbilb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ecsygpon.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3itcnovsk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rkghdswq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wczxwfzp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fkledqkw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cfmuyrkm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sivoltck.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3rklijvxe.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wmaoeubg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3hqbcjxtu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sgtwpfmw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wbxxbexm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hxbonjue.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3lydmzszl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3smbjkons.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsojrqu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3puuznjpa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qkmmnkji.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zfvwzang.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mofgjpvh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ojhhdxrj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3aqxsagyq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xehmdkev.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hctnhjuw.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3renzgzrv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tgnqpfaf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dqsvuxsw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dzvsjasn.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3vwwfgmqj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3whnrwzvp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yedxoggm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zsmdvoiv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3modmpfgk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3syxayhis.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3okkxqxuj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3atfqmrxn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3eaxuepbm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3sdfqcmhd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jqgijkvr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmgmehjg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vjygbxki.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rlyuhdrk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3qfeakxog.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xmemoskj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ahbkvmxv.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3mpqdxlxo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpnmuxbf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qesnsvlg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qdenkzck.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nbuxetqb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3iwhednxb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vfttgsoe.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dlpyfvvs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jeokmtra.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wgtyhyzf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyftxegj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cnwimzok.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gxvycgpy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vmtuuntp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3luviamwb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rmhagbkj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nnryifem.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yuobvcfx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ypptrknh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iadtoqga.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mvulpqgr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gtdjlgbx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3clklzzwf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qrjkjtnj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uvwsybwh.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3cavzmfmj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3iirzmpbz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qfforecf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yivdonmu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ievdcgvw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3giwuaoht.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ijiqyxoh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ktbcjgkv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3chtdlbpb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wknvrkae.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lqilwmgs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sxidhbht.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bmmhnaie.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3tnczkshu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wahcfavk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3layscqxb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hunzmvoe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rmcqmnhb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lbvacshb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyjqgsx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tlfenxcx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jhkousyd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yrahoyis.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ecyphpzr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hjjwsexg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3elxyahne.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3yxrgkvqv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sntcwaur.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eiwtgrzp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3oyleuuka.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kckuthop.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vrwfdqfp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hfnzarxb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3gwjifmld.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3keuzxfbx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3otnmsdwq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dxnpcgmt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3wsuebnvm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nmbxzssj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gnqqcoho.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qocuxbtj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3rwaompjp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3yjophpvs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kskhttrk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lhwvhsig.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dlxiszhs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3bzarnutx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gweblnad.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ycmcgovk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3btklgwje.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wclihzgz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kmibknfl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3msebuupq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lmwkzeow.html


<!-- 参考信息 -->