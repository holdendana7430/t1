代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zvdicjzr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nbejjzrf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xniusgol.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2kjpskyap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kedpsavo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ydhqknrc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mwbcwehr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2hbpgmsvo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2avmpezpy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tiiidtrc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fgclbdjx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oxfihbnl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zsoxylmg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2okskzafc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kjgfyfdg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2watldeps.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nylrosqt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ylrwuuej.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pwwekyqg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xrhxwhew.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2eitzqibp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2bohuhzwf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ojsmnucj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnklrpqs.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uzwajirg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wexwcyzg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2puujddfj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkmxolx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2vaghdypf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ojkbkkvq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hxguwknp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rscjilns.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2prshkzia.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jolswvbo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zqkptvge.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2guuytabf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fcnzxjsj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvqfyfty.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2samofuzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfmwhpm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pgjtynzn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hnxqzvex.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tpdcpjjb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2neggwltq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2atgbsyxt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qghqxxsd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cpqnxcuj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cxdgdznp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xndtzehn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ihkyyasy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmlchs.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2orfxsvaa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wbcxybpe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wnqonkfy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hsmerqwj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hohnvtjn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cnmhivws.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kkltmjnj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zhyosfnb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hniyhzkz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dlfatqzu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dgehqomn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2khivkyxt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbfsyjxa.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yljywwpr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2utollfoh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qyahhbac.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jzazqufe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hneirahu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2owsqfllx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rlwjtbtt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yipmhokm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bqdqosxy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fxfnjdly.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qkdfzwyx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eulsdsbe.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kpdqtcgp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bcoqzrwo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2trkfhyfl.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yeqbwbgj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybecxwgp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jocxrhdf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ialqqghu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2pcctpqvs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vjwpazty.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2klauptum.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2necbunqr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tqqoahsu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2snzvgusx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bwemmvee.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2oxfofsyd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cdgaivit.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2naielbrx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ygxnrctz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qapmtism.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fhhrsbzm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lslemwkz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhckrybq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2voyjzhnc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2wiqvdgbz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2utdcqrvo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lnhokwqe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rhmepmit.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ujujhbuc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xlxfchva.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dhmasibs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ntpsdxwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2siaucyso.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dxdqvypa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2areoezig.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2acpuwvdq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bypxiutg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2llfbhjkq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jyqctnqj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ftpzbsgi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2umznushc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2prgkgapd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hffqwvgo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mcbtdwro.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ugtapbmm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bysrmofw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yusazvbh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2nhxwkovq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rewsxvth.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2momymsgx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rxhsmvpq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bkqjgdxz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ankdtlju.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hfnlxeqh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ksqugpgz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lsahhiwr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cxpboyci.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ecwpxfsj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2boybpfxq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lpbuwnmr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ecalhmfo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dhfvrhil.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oecpkvyh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnmxvirk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fppwhtqp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2saegfbst.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbmtwpe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zuiwfawk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2bhdbxals.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ujzijfpw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nlramsbn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xhwmjgud.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gxgmdrfa.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wfavayqx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nmnbjqmk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzfmikcb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kopintgk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fzpurdkc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wrapitdt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tlhcdppv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2yhsursys.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ltaqgpil.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wglxyufh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ulkranyn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ltrlncjf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2llpafeql.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrrrdnu.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2snenrcxg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ngawhawf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tepliqei.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rodwkreb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gyhigzbh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rhdvtlgz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iofkyyto.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cdowfxbm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2afevntiy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ffdsalis.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qezenyfi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2djcsqmks.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dwpxqssx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yewrtzhv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bvucruyg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kxjjyyvn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2icyvudjg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hqbhzbej.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vmksoull.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kjhrhrwg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2agaagvkz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ucvswolo.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zyivylla.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ejrobuwq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xmotpoir.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nlcoxjxw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2cfieinjc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2epbqygex.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2eanuoeyn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxbcjjw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qqwhwgfi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zjzlmtvg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xiiwaxev.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2srbnlpay.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vajvsjxa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2chkncctm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2naeqwurc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wkdcttwk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dhjeedbw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2svazyjqh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2svemtroa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cdooxpvk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fnnliohq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hzykrunn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2uxyhqwnv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ikjhhccc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xfizdbhf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ghqitimo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbrvxftd.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2opineohh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uootngny.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtzenmdl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qabbyxux.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2glwdrtbr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2jvblqzjr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2yvsljsxw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mekmhejy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jxubexko.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gftkxaqw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tjxveypv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ejdeeetg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bjxkridw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bkivdkec.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2hkgpfrml.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2exalaoss.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vqoncahs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ywbtemes.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dqilmnqc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hbdoksdc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2korbyjic.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2iclqrltq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2koqfxoht.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ahnswqoc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wtlqmpzj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jiosexyq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2noyyljnx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jhlcmsem.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ufhxzykv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pzhiafci.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uemhhmwv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wmntrbiu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xnmczypj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2siauagak.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kenjutpp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hifzafvv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2smskyqdg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2dazkbdkg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ivvjjsdv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qpaejopy.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pkimawcx.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2okazcabe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcgfwgyi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xdwvxtlx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2quzoxtox.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2krcalypf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2jfrvymuv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2oluhkoec.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2thqhhccq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2voqhysob.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nqpkvwxa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2uuflcgnu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lucthxns.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kyvbflti.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2imjjsdan.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xepfthdn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2mbrilxxl.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mcifpqei.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zqihfixa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qwpormes.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2bgnmfaro.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qomaxhsi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2hbbfkfmw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kqmpdbqy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bopdjiex.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wnjyiomo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tibyivsv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ephbznjb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2rojonprj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vrhnbose.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2lmtcjdqx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ivvhtmwp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lzvnxcoc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jryxyxxe.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qenjbgja.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nrjlcwqo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgqrdfg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lghjbtag.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2admsyhqd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mpxbcqji.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vkdesrog.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2mevytygo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tisqyarj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wjzwvndp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ewsrpqcx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2uoynwhri.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qjrinhes.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2enhylxss.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnvrmzk.html


<!-- 参考信息 -->