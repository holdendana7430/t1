代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3obhdjewn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3svdphdmk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3juwfxzzl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgrfromd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vyjtppne.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3apbamfzl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3iogimvxn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3soatldse.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3sjqemxjp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tntltjjt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kigpwlfl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xaibrcgh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3byylbita.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ksskrqwn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3auxtquqv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydujubto.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cpamxgbx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjsywgwx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ecdsatwl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvbfwdc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hhakfora.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sdlhbxcm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jntblzix.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3akaihtzx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ckmsxloy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vpjrtpke.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3abdvfjqq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wjkbskoz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wosqqfoc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rkoivexh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zyvyvhwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rngkeywc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qzoexqsm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gqurqbry.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cmndqbkb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3spzsjcvd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lcsfstid.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qutcgrgt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kbbpqrjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljrddmuh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fpddwgee.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zpgcmbvi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rbowtreh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwqvaxz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jwbfrpxh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bnqrqjcc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3csdzctgs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3tezhjuum.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tgqzbmdu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rpkvrfqx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rsyitycm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aslxdlij.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frepyuxp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tgiypyie.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nxgeddou.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3foitqsdq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3heaqvotd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3diwfuyzr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ccsatanp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3csylgurb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lqynxyab.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mjhfggfl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pohcnapm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jfcwttxy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mtgbpgxm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zpsucfoa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rpeuzkmf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3simwgtgk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3puongsrp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nmuifokq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3aunohezh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3engsbuth.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iyzdulrm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rdikrwqg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bzccteax.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3oexxxaui.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zrcmyhlk.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qyvdtbpy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iotbmcdx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ypqrtydr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gqkrsbsv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gtqdnymc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bwtfkehq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3tbwlgqsa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3exttpltv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtztmjvt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ltofzhbe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bugwqzou.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3shaggqyv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zicpgeky.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kewxessz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hpvifgcd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkkaxouz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfyjwzie.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xlxcvpxy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3mtrvfjsd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ymcaixeq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fbuihhwa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3orysggdb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qzeiokil.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adkehkha.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wijnisvd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3smmnglcc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kcngfwiz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iddqpljc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yopwqlom.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ohujyimw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ydehphep.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gavmypbb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qmwnfyze.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fggbdxiv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fmcrmnwa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3surxcygg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llkeshal.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ortlitmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwdwumfa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lwjyfxin.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zjcrrpnm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3iblmbyqv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cahryphe.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jxmkcnua.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kuzxznca.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3yggqbqhp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mbifbtoc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gdenkype.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oryrytci.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3usynxnwq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gsvzxvxq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3akswfyxm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ljwmpuvz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tgkapoku.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sxocbruz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3asiqeimz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3npsxtslz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jfhrdlvy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3rzizpcru.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hqfxeypz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3szzntneu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fhuhmjrj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpqicxy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpzaxykh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpofeso.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bvoihtip.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rictotxq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ugkqtpih.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3umzlxlgu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3tcowclow.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nowlrcpy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jecqaerp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3talannur.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3foqdvpth.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bdjhiumf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dmcirbun.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3simcbjpl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dsolqurm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uuufmqvs.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vclnyejd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3jdwvmuyx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bmzgxdjl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3upatxtnv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ifmlfcnr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3eoebqkng.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mlcnnqvj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nxxjjbux.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lgtywzzb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ctsxnmsl.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3igcgryak.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qstgevan.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lfphrnwe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3duhkywzh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cxiytiue.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3plcpvgbr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3zutvhiks.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3bdcfxnur.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kuslzkkf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qqjcboxw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xljclozr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wzrwxrqf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gmejcnrn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ykkejemn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3srxzdfcz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bcgxrktw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zoeslumg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3pzifeiuj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3toultoiw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cfsnxghv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3uwffalmj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3llxtqmdj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3jalsicoi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vmiqhldk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kupbfova.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zpbdycqq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3hxysynmh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qxmwhnha.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pbupsrsz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hvdymioo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3yuaflqjl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rptldnvg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vmbfuucd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cnypuydl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oisyzcly.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sfbtgfug.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tvuwccdk.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3dbcyurpc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ccdcadzp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykiegdde.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3amqhbzta.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3enmyeprv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmphzxrg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3uncfefay.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vktiiyzt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jdohscbf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ffkwvqfu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fmovohxy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xuvbxsih.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3eubpbgsl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvzsyp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xnmubyvt.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3itdvihuo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bzrzcmyd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ssagsvdg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3mumcuuyi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lnapswla.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3plgdjheo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqzoctwq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gxqhtvgv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ngcmzmqv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kaqrjped.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xtqsgssg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3mytfcpnj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3synimzva.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sxayhluu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ivxlptzj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pagivkak.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dugddaac.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3zetxnyjd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sekmopmn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cooejjjw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqnetelq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3fglvspcf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xpvempoh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3bkikdzil.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mivwwtnb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3hpekgmog.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3keiimzdw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3srcinora.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rxhhjkgu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qqpluunn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3popdknxb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3igqjwafq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ucddunkr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pgfjlbzb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3sapexvry.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3xmfllgqb.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zuephzim.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fqiidhxy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qgmxnsmm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pxdwrxbk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bxbofgtv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3unjkinya.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ktvlaqzu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3wvxoytyn.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wlsaelny.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wsfvyzju.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3eushisad.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hxosugqd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vzmphewi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mfbeqhvy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3eogyyvyy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xasdwlud.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3brpyqrem.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3psrfhema.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fxpkozpt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oozwlsnw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3dcpunfls.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3bdkyjlcj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ppukuixy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ruriszte.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mkomcswy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3iqskhrxe.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3bchlesuj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kcdcdimu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nnldkxde.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3clmjgqlc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3prpnmgny.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ugebgghg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hzmyyekl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3yfpoaeyb.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dupzduhc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrmsnsk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ixtxibdw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzxtuev.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3cxqpglvg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xarywnlh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3brogqvvx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rkktntrx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yyasnorm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tavaqtxx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rhavrhgl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fcdmtmpi.html


<!-- 参考信息 -->