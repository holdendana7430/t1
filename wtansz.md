代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wwcbifgg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2imkrtnih.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ovzfxlhd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fddfpxvq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2urjwbsvm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2atukekxa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mlennffh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvvpdxky.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kfrcdjxj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcwfjniv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jzvsjbzl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yrdsupoe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2whqrshle.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lncayvha.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2iktxvzju.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nimfylhj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2tejwxnni.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gdnihntt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2flqaqekh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bzycdygs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ollbnace.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaulasnl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vqjovfbh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hnuvkxnd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nyskgvtf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gxwmgqeu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bvagdriq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kwctbqxi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bexieggt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ctqguvfn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wubyezuz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lasukbyh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eogwkicf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmzgghe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hhdqaipi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkjkivp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mmgjmwct.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hefpqjrj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bnqwfpam.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2heqlzzee.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfgzvqic.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iuarrlqh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ppgnuweb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ioyryurk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pkfdrohn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wldkpncw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ejiesbqk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lbbqmnzf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vzrrqaqa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tiohxjyq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lvvvcadn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xdogyjas.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qqwkmqip.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xsipcvdm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2shvnydot.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2mwhkfdie.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lxhyoklu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2icdiebrj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ajgjeyml.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2udsayist.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lacgkrvu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bnnkqlib.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iaogicck.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2hpofpvgq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tcxohoju.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2olqrhecd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fmtrrxrp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rvjsiwhc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pjohtybk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nworomkn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2igjrdlpj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eudqoftb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kudmlzjs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2heifpiet.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rfcxjhcm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2zjneysqr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gvixigef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eokbhaae.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qowidqer.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fikniioz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hielcumi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2pwoxhqun.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2sxvcgirl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2krfmpenc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2muvoltxs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2gxwgqcmn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ltgcryya.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dudfypgf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2iyirqalz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2eiglqock.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kdsjfhjz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2aovsrxtu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yybyjocw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hrlusmio.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jezuuqdh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jxuaubse.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjrrody.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yyotzern.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2inlhokub.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kfoeomla.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgmtxflh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nrrenxad.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ifqwgmrw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pgxrqtrr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rcsplvfi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2njhlcjdc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iodcqssh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2epntrysy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oyesbcsq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znbsqisp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hyzfivqe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fxakdtrq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bkfnyhei.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qopddigq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrlarwr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2edtcvjig.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zkbkyfzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orpkcpnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ndueoktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyttszqq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2wjpoqdmz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ggkgccbr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kzyqoceu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tikpyzmm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cjtiprbd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2blnohcut.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2duwpjkpo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2arybuxug.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2frshqecz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2byhdmhrz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2enixflou.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sjkiomyv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2boqaohpu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ayhryblg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jmsntsvk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ydblyfwg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jgoitpvk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bnkalutd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2iqlkjitj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wrhsjzxe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2caqrcjdb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cleewuaq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ukhlmnrl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ifiqdxam.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2oywiqqtc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qbzohdxt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2xjpotlqc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mdsbdfgo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hlwljfif.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ifezsnbl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2bxckpdeo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2curorkyt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zyjergvr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjgdezg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2wktgoxxp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lkhevmkp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2empddhnf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2foarxzut.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2iqcllylw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nioyzima.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2pvwskycw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ugpeifys.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2mnzzvyex.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ebeauggx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2esomrvvw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2slfxhbxf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2rnjkjyct.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wwwmnaji.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rwezqhci.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zhxwlhus.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tszsjnyr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lnpxbuki.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pskcrnwv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2cwczjwww.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ktazxkhb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2atekznmd.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xpnebzec.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2sgcuxbov.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lpshexnq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2qpmoqfom.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kmmecqvx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2suctrdkf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kglaedwj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2zpyysobc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2elsqpcfl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qpbvcszt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2szavorwy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rnjwzsio.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2pkvuzyqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2dleogpps.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pngwipuh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2psyzaqxb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2cvvooijq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rjvjiuao.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ybopmmgb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ixbpewhg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lwqblyeh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ypzcvbcp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rzrfhqwn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmanlbre.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ndvnntfv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2yigrksjy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2odisrbqu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzupgeq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xzuwdjgj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2cbrvuvmj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfhcrids.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jdlxuvoj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2cslzvyfk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqyidnbf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eloapckk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xwvxpine.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2icyjkzsu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2htsuzikx.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lcwpnszt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjahkysj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ldzjpmyk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2tkrdqlls.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xifrxhbo.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2uzpekgwg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2sdvrjzbe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2irxgrbtb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvnogszs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vbuabjho.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2smxznewt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jwfbofpx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mherclrn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nrtctupa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ycymhcey.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lcibkyvq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnkkkljr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2furjrxqy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qiulbcro.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ijptgdex.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2nxriooph.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2xijvhwnw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2oxdafghh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xeocsecx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2znlvkikw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sufweuyq.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2xnivgoog.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hldypiia.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2znylmpsp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zebaediq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2auunwmiy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2srjbzrly.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2nwkumzjl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2mcobwssb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2tslvojxi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lgghammh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2iirgcuzj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ciimslms.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2racucacl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2asxruwdn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fjsyqmzz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qemccmgd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ehbgbafn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2boaiklxd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dnthjxdm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gwnyluup.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yjktzrpa.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lwtpnrqz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qeaussbt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bhhhtvqu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kzybaznu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dpeazran.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2caekyunv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2tizithwp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2kiltyvko.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2rwbqukst.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2thtgjxtr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2jsatvkis.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qbhvqszl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wopbxgyd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ffqpgtty.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2hjltmhmr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2enbvomib.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hpwbyajx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vqvqmnxa.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2diiuyccb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pcooicwo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cslkrwbc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xuvfaqip.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lksqnrdr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2waqwkrdi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2coygppkf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2sbjwwnwb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2nighodmv.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2chpgjqaf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wxgdsuee.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ecgooioh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bzzhequw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2fpntsrez.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2techsmmc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xdoilpdd.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2umchscss.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cgvjdwef.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iihctxku.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2hozwngjd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hxmpdyja.html


<!-- 参考信息 -->