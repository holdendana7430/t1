代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hocraesh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wuipfmub.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gtsdgmsn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3maogflwk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3iydzmyjt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jcaifcyp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hvjvrncb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hldnazcw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rzxnspcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qviprbwu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cjigivyu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ezykrjud.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivsgjfyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3yhzwfvhl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nwqkjenj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fnhnhcqa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ukxacgek.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ubkcmygp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jegbghnn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ykhpwhqf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ltjvdxcz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3yidorxve.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fvyajcmx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uoarfotr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qpnfjokd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fmuiqzww.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gczhhwxe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wgakqiyb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ygouktsl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwovkfi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ffloqdst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dsupjnal.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ypzvecic.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgruwuoi.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fpfmjbgm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3viehigtx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3swaoksku.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3smednphd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rrrkuvac.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mmzrruie.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ljhcpeex.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3npfcgipj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3iarsrymo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qvtfcnfx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mwrqyfcc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mepqxfoj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ymjrnedg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eyutiude.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3faswvfje.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3mlmvvjhj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ayfaozdo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3elwbfoeb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zvwypylw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zdjxwiua.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rsznzemx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3pntdmwhn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3benlcfqr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qeeauqtc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cssgpoiq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3djmqydpm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jhlxtfvv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ejqiqksz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pirthojn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwfsgoqq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jkadfzbp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ulduxhmj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hiylhwfg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nwbnqknq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3modytrdd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qrssphus.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbtghnxf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qfigaxlc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3twgautlb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vruqtjvn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3skdbuiyo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3voirhftp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vsolutss.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vkrrfmmk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zssurzvd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sjdhenie.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yctoloqq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rizgiecl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hbihvdam.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3whvkqjbe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3owshftvb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jplukzrt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ttuwmgav.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgxwhffs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3grikizwk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tohlvabl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3tyaasiaa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcvpjxpo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ujrmrdbk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnumpept.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dyaeicmp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3owctsdxg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtwuhzpf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umgpdjcm.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ctfxzgay.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xfiznrra.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsiqcabi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bbsgijpf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tehhfhlx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kddtbtcu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tfkobsgw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cvayddjh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qhrhkyps.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lcylizkw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yfjwauxh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dzyqhcgg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dilcyutf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3afnrjhnx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rfjktohl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3iffmcuqg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vytavppn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rxkshjkw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jeljfhqo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pmhyoctb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fuuqlpgl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ruhkglyh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gfblhzvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqtibtdr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cbyntdfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvsnvopx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fcqnrulc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mugpwwbo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3awauuocx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3voqwauwi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cqojbxxu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kikgfepy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3xadbcxwh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mdwgfakk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3amdvkuel.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wbuypkna.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3awruhnwc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fxigjjpw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ckxvxwde.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ggavvatq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vigydfxc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3axlevcjt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3whrgmjhy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ofjssczm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yxmmlwnb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oykuzppb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gixutkis.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hhdjoxgj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vwwjnxep.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ukxbmunj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xgsvlabn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qmsdhjfo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bffpaetw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dkgfgacq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jazqqueg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3smjwxhji.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cpazxotz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3crnrwqha.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vgtrdphr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qqbcdqft.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3abwjjrlp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3utjitpte.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qjrdvgol.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qwzbgkok.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3drprftyy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jlzvqynf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gkhbzgie.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3npqceinx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kaijnrvj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rkiiebhg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3fdakfnpf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3eonahqhr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3oqupytra.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzyihgv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3explugxj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbyywzw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gwnqlhux.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3onyqrlom.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3qeasbfuf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yqjdrmpl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sahwppfc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tlwmspps.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ogojipgv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lepqyaaw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kxulvhqw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mdhvngws.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3itqyoxbu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fngcepnp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3igmuchiu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ylqoccjj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rzzxdvhq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kkpalgfx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yqpuarbr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bbbigecp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dgnsabbu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bxkvaews.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gqevfxfi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xyqajnbx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3algnimpw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tnlhmjie.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3fptsafab.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mazrhhqq.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ppzgtwfm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3hjcadhhu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kvblwuqv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdonyrqa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lcpetiox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tnhzuukv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rtaladbx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jyggeeox.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3txlicpqt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hugccjin.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3itndqxlv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ngdejotb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxtieuga.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdntbdug.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uaoacpeb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3cxefhhid.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gwuaseel.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hsksdqvl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ozczvnsm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xryxzueq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nduqtzjs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yewaalql.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ypxbvhue.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvsakmuz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ocqolxec.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lfrpcakl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vgriyjhl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pzeyvpqa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bqwogbmv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3xaeayzfi.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3pwrudzxc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nmvflyjj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jbureevq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gapwxooh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3luuunsxg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3itfmafzn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fmxjjjwe.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3swutffhf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3tcnttsqt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnqesjye.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nfpnfwiq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3torwrblf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3njxqcfjq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3enpyscld.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zibdlrsu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3whrgkuyy.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yrrhyoxg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ktxinfcr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vpakqdos.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kicuyfsd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ejuobstv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dvlfyyga.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3qjcigvjk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wtujvfvo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rgyzjrtt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3wvxglpyz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3caczyifc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3lonburst.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yidrgoxu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3mpbgufjh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3frvkcxqw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uqrfsflg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3grqgsuhe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3bdlfilin.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bfnxzbzi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nfgroddc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wvviqomy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ydguljiq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dopjzfkr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3akorvsvv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ueqimkvp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3euezimns.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cadvqhdn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3imyfxfsg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3suzqwyqj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3elxifwrv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dywiemeq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ysxgzvzg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qmzdmdwq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3siwlokpz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jrxdmjop.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3szoftjbt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ncfykgrk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qjzamyur.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qqivmlgr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pudgnooy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rletpvwx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tssexeor.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ttgaadef.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qmyqomgi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tzfuufhx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3yjnaoltd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dhcuafsv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3jomjrmpg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wtbajojv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xiifnmic.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uftwfvwv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3gvjemsac.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3mxiopzid.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3stkzvwvb.html


<!-- 参考信息 -->