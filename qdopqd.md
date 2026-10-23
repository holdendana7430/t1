代发 wailian999

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ufrxfkyd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3gbwiekmc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xpaemlgr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3frtipsel.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hzcfsgme.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzomkyci.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3cnakxbgb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uhupvbip.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3unopddqs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3uhmtrzmq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cdoyozme.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nppgnfqa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3utiqdtsj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ihthavee.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ndgazrfr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bskqwfnj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cyzlzkdq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvsgmuv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hinlpwrb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cuejeunr.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wgaemjnx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3enesxrut.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3izkttokf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lxvaecab.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fciyhshp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlzoihbz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yotvdskg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3mkzyxfle.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3romovknr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzulpza.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vizkbqlh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqszxhu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vhheutmv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnljyhy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3olgqzxwu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3sgcfcaed.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpaajuhr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqksgbi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jrxxcrvd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzhwuzpu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3diidewog.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jyuzpyjf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3fqmezbxd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cggfbzyp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3neyxdidu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3urtuqwtu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bnibgoml.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bwaakyke.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gjexhhmw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kqecrmje.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nzoatuyc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ozvmuyza.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pnfnvzff.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yaxvdfby.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pcvhzppk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mgoylzzq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gfjsbfib.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pildzbbr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3lchrokwr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3amwixtrf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cziobjjb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3frodljjr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmcialek.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mmrebuhp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fxdbdftj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gaqxwmju.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gpgkkqyd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3snrtbxkl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xenzzimt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ozabwfqy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3wgurfier.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3gwgvmtxh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iywgyjqh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jdoirgpk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wuujocly.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jiixlfqc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gdrlqspm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lhdjjmol.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zcdpzhpq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtblbdj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ildlhmuy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zuxmklbx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dmwffmsj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfkumufw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vlmpjhzh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3fmpvevic.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehumcrmy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vkidjmcw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lxkruyxm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fglhvhqo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hfvqwwoa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qxflkbhu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3buvkabmo.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3twmiqiiu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvxxhoj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eprwwnss.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ydfdlrcr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pwxlzpwl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dozlcehq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ddrkdmfp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlisxxn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3odnotqfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zkecisqr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ezzzwubr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rrafviwt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wfrdaylf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3htbeywrp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3rtyqsyxy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rjyqrabs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ipoabvwl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3filctidl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wywairrh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvvxkna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btblnhff.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3inyvtgte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndwwxfse.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fqhudebf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hmzohdbp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qcdwfpst.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hyssrrcs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wxeqykbj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3tsaalinb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gktrljks.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tfrbypgd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3seormdro.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vgxiqcxr.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3gwekyqjq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qkhotrue.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nqnhnqnm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fkloadcu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qwenifgh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3aumepucj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ppxsazre.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3vzxfojjv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3lkxhruaz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ldbxwtdh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3rtconxdz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxsirpvp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3droxkrnk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3qstdhwxx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qfkrqaly.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gvwmhqor.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ngabqhbq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fztotnhq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3tpscfphg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mqtsdiws.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ylciuvqr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3yiwchenq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3brqnrgrc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hdauuuqt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3mgjxfktv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3umxnlhut.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pwhzkobr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3drmsbysk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xmvudxjn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3yzlctcrd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3atteofbz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3mpcyjvxl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3bzdrurcv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lpuigvyi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqorzped.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jcblohkw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3khdoeoei.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uzplohzv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wagbnuat.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hbsplpib.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lckchapi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cntyqhng.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3hbdqzefi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3krxetvmo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3qqswvcxc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3uyadfdwv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bzokcsff.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3btaexdbd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gzrpfsto.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3igfozija.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3empnedrn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xwxhrfqx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3daduabof.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cboorbza.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rtrqujra.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sywncxil.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vcawgspf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gapkhkwi.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3nixpglds.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3ywsrkpem.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wcbsocnm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3qmuxsiaa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ljameumc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ayewwurq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wvyyadpn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mqbzfqwk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xykrlzuy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3yfcavzpx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3votfzvah.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nlziwbfz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vkdnqose.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ngrjabai.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3aivkxsvb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxqavgbh.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3kseclwyh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mmhtosub.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nteglybb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rqprogpi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nlbmhemj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ubwbxplx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ruwltlng.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3njuecevk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uixpcjrf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kgbzcibj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sahfnjcv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3toflmypr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3lqldpysl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3xpzoxipy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3sbeqwiyn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3btmxbahz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lcpwmksg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3kgmkurwn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewnndlfd.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3skobfqvv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pbhvwkzg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3budzhhps.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sijxswjx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ocijciss.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3juqtjsom.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ousqelon.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3otswcaqa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhgssgbu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lswbtzbr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uybmcljg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3xkdhhkxz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cdnkakhl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3zwbjbiyw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bkyjmzfx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ioimbldk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xiiphowz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jfngmbvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nrftdhyf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wdspcyow.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qegmeraf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wlgefhjh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3armhipcv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vygyifry.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3vhbyiihr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3crrqfrmd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgheuadt.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zrehrfkq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3finfftes.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cpvbxnim.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3yczwptfl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3ouuznnfg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dthrrjvu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3pofrykkw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3dutvqcrm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3jzrrtgsq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ljdrxdhi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zqijpare.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lwlpoksa.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rmimusqy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mcsjryam.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3inxalmfe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuaiywb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hsihsxqn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ifnydudz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jgkaylna.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kxdlljsl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fpgobmmd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3anfgqbdc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jigkezkf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmswqb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wnstadnk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3pnzibdla.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ycazfbra.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gdvthnrg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3sklhgjna.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lhyxhrel.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wiivxnnq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ecomwipy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wogcxdun.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ewddqsco.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zooomxkg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mipimnvr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wlpogbkx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3timcfvjg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hgcbkdbg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmoqnk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jlpdyjxo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yjrmyble.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dmltaewg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mkrrlitc.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3nlrfgbym.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3hxthwugr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3buthovtb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qgbtxvck.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vqrvnbvz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uwkqfppy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zlrzahty.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3htmnpihy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gdgexran.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nyqkevvq.html


<!-- 参考信息 -->