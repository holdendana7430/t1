代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zpboiqxm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cpdytzbr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3taglagfa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3omxtmyvi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3izjytjor.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3llyygoul.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yxxfspxl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfoepcp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yauvvtvs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xicfoxtt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gezehuzg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3imxqqstw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hkuiicpj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3liuyermz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwywcp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3fhkytfua.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ldxfilef.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ybwtxeeb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rrfcwuaq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3stihgymx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hhadmrrq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulbamoon.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3akmligig.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xkufgmwk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gdvggjam.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3chzsarub.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gfovysnc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mfdtwdos.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3sbzkngsw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gakpdauf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3avlwnjrc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3cwiabdzr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nzyenwjz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltltzclz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hzvenypv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3jkcscgtx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gonangnw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cmveqtxg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vaifmkrw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xiheuwaf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3njsysiwm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cgsmlqwt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mqcgxxia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3imuascdd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3viiydndp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qrwvvkzd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qprbhneu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sscvesur.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kyiddsrw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dcwlmijl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yfhcdear.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hacnuaps.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3yzyytrwb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jfdjwlfl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3svxonsyy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mytfwoiw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3obyuusom.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mwmhfsdt.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vmfohtzx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cowfwwmh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hcblswhm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mkcfqtdt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lwwxfrtv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tguptlyz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jpbuzimc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ciloztfq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yukplyob.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vkcbhyuh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uwruucwj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dkotfrkn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xbgslvcj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ybvanwqu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xnnaqgwj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ooxetxyg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3yncyzkmi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3grtyfwik.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ilsqoovt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xycpocdf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jbhzsqjh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hpxkgztf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vrhkbcwd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yrjkphew.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dyrlfqab.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efemcavq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwzbuk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cbygdmdo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zqeklnfs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3guhrtkhh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3leuuxglk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dptxpyim.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpikum.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rebupsgn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yuibwqup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxqpxfj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iszzvmyr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xqpmaptp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uoepiyzf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qpuqppce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ikqmuztt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lltiqwdc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3atdiqtwx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dliqniyl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jhtbwjug.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fwmkzpwy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ppnxjqzd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cjckvuzx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ctqqndso.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3evityznn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fiskalle.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ctpzsbxb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3afbvnclh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jnqgacmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hjjrrims.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbumldsk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wvodvksr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lwmlhqbs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3spjwqphz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laqqiogz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vpslpgvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emisdzxr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mwapmwvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3teufdfxg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3uamiyuzx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jzmscaxn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jeyejjva.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gohopeki.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3elrmvgly.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3udelgpow.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3phpbraib.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rgxhmsgy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vfpfpgqw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kvdmteng.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3urtmkqdc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jesgpdyf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zclyhuhd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3xvagcxij.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3latywunb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bmppalpq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3baqybyqv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tkatvrkv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pmcthplc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jqeyjoym.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqxbqjex.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3efxjvazr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3oabndtuz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ytozpyfz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3viylmgtn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gayasyxm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3amkmbigb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3lrwrwqbr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uljbtocl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gfqsbjdh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yllruklo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jwceycuz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zxhcgaut.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mcvoeawy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cuegsgkx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hofloibh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kgdalgav.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3popgudzh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3gpjqpxdf.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vuhpnuec.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ugklymro.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zbwsjcuz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fisausvc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hdlvknpl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jtlvhsrz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3icbqemob.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vaqknene.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3voagpjnv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3njfmccwg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kyphfpph.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ujhrwzls.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qleuzxnh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kbjzpcok.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3orfgotpy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3smubvppi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sapuawoc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mzmivtrp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3grdisipo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ntgzjodh.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3aeyotqwg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3autigsci.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nsvaeoif.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3inarnsfy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dxxlvhma.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3otyhnluk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3usiurprf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hnwvqsys.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fuusxkor.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yvmyixit.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3joksuyoj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nznvhjii.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bwctizql.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xdbdlbhs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3puxlmjyi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hufznjif.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bkxaqmnt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vwxgffpj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lvzgzrrq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wabnywns.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3otuarrlr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pyginvan.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qitbfbby.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pokjlyfu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bmsiolmm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3edpympen.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bwxtuoxw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3bwcnxosp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydmndmyg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3iltznetx.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjehlb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3bdvmgkxh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3onvydhwd.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ertkcxpv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tmexvldy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pszmbtpk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gfgobgiy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3aljioiru.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mbnkypwb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3zyliplaz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vmunzooo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rzdhygfw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vccavaje.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3yrwonxor.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3sbhffumg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bkchtfvb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3seywqqzm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fyeiisnn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3eagjlebq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ipuybtgm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wxifjfsa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qlsdwsep.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nabssljh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3pgxwpfdl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lmdivolm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tddjktzy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dhbvwneh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xbcgbsgx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oygnjtjh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3gmpgdwev.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gddzvhzt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3huisodki.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wfrpczhy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3cedvexrw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3leijsjpp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afjyfxlf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3euhlfakd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ylndjwjx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vpiebchh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3phhiqrsh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqzfgn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3idogsira.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ddbxucec.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3vrjsgwwb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3civqtgoo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3qpzyretz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rvhtqgne.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gnotrnwy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qrzngisp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hbmdtabc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mgnnnmyc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wpzahtyu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3wlqmqcpn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wknguwhr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zhzosixe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3efwhnfcc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3gunyaywa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ajizmlmm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vhpmwrem.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3seatjetn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ugbxicdo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3csfbqrgc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dzylkdmi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hhdnyfzy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ouuzdcal.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xutrqoxt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3oduhxewy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3pfkwwhyw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3soaeauja.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cyiachdu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mttrazwv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yjbftaco.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzdkvpb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fsdjiqtp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fsblcqwp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3adyznlqd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bfmruywm.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3tdnlxbfr.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3njnlscbq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wraffcwl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3eljvzzfz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dyrckdsh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wsfajycg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lcdnalfp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3exiniagq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jkilapbu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xwyivmsm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xyufqmoo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qxrixgso.html


<!-- 参考信息 -->