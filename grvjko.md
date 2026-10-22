代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cetxenam.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wngdragg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fhcaorxk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hvfndrtg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xwisfgfm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jogzydju.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2duqrltuw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxigmimx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jtszzvhz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jnonbdjw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2muomgiof.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qepaiowa.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oziypeab.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uzhbtpni.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xoogmrty.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2janzbbns.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2maetjvsc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nmjndxtz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fqnlhikx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnisff.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ghfanelj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2memhvrif.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dntnnuai.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ehzdawqj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2npnbauyo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibootjrx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gcmgzmuw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tgdembyj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hswnvlwk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xkbzjfow.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvzjqpkw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2djnrcvin.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2uuvgadat.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eyncllot.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dlknuzxj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nweompgk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2iebbdsqp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qtflhozk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cyfoyhaq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pcozrjiz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gatjomit.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hidemrpr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2afjgzppa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2myqahrlm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2iskavhjn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pfqfppfs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nizaocau.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2njjggiyd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzzpww.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ratnnmtg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vvkhdjnz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uirvreux.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2legmloei.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sfndylpj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2loagvblt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kyxbfeya.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gsoanfug.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hhjncuvt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2paaawfyk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qunoesel.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2itanovdc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sxsqxjpq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2khmubidl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ihljupnn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jbubizuf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lvcikahx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rvdyiymh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cchnhgmf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xermdfhd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpigvynk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlktrn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2biycrbso.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cotzfnfi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2somfqkfg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hnefbzwb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ydbsvnef.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ingscusq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbofqdn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ubqvvsan.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2smfsmoxj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dqtukgrl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ybfqgsez.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kduqmsep.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2skzpvytx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2imiheluc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pqqbgsvr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2gbjwjook.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2weyhoqng.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laqdyyrf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2oopanibn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2oprmzuvz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djzhaeoe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ksorfxte.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ncbftkup.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xiogtkqh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2sdbtyiqy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2brqdjltp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ddvgxhpo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bvdabarq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2vmhdmstj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2srefynba.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuwgtdfj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2opaymact.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mszcetla.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lhiraovn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tulmjtra.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fhzzwbxm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2thegdsoc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cxjvitky.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2flrwhfqo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2khgqruoj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dkldpckm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kzxonnnd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qbizcqpr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tnxsvvmg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2enkmjjvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2beeysnub.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2loebmbvi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gcgmosqc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qlwtsxxl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pprfndvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmpcjwhx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2supprmnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uatfkkvj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2sazeuzxf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mwdjtxsl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zijzjujq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kosdfxja.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gkytnpez.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pqshcnwc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2irovpggu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pejrmakq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ospflwtn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ofohehps.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2sngtrzix.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2raabdahn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ynerriku.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ajmfmmve.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kwcbqnjn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jzgwikvk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dtmysnnu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2acxiicne.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2epnoodom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rzhxexxk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cgztwlbs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2zfobarry.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ztiuifjs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2edviosgj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2owhkpqaq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bezgjyam.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rpzgpnda.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zevkseoi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dljlqbmh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vomnzvdt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2cwjmxtnq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zzhjhyfs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2djwxtkit.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jogipfoq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tdbsltrv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fkjgbtcc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zvzvlznk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbzqcvot.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tzwqqdcp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ilrexygg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2koqwsaql.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uwkwobej.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iixficly.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2pxsfjzmb.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqhtrrgp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2yhnnbnnp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2pxksyekq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hsnaavmk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2pvzixies.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qealnosy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cqdgdjat.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yzbvebjo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2oxizatei.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2lutmjeig.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ojhuvvso.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2faqstuer.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2kopyckwh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jmelnshn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2qtuiwovd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mnxulohk.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2mvamwevi.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2bnelnhtx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2scanckly.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sqdfdqah.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2sqnrsznb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2suwazwjc.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2qadlwgja.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2otwntyyy.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qtczzaud.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tbsentrq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2enlmbajd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqmcuky.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dobztwdk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wprxwucz.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iemympyd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2umzunrit.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2dwiemmyp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fjiiifod.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zinewihx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyxzfaas.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ymrvmtwh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jhhdnfme.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rtincqau.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2etxgwcee.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2exjlzeua.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rwkisynk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2qeubxhay.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2gfnyolfy.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zqeqimjy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfvjljyb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbonvunx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2kbwzwopu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mzmedbwz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nkxxxlue.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pzxwmuom.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2qazhhcdd.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2kufypevi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2imalpnou.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2wstyuusl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2eulndsfk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xfpboejr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jvgenuip.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywqbultb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kvbiqdxo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2upoiosqy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yqoganbx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vwqcziib.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfuluiw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2jnpresiu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jxzbtxpm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2zwmgebjq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tofrtlfn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hkkxxhhj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zsicaofq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bcwvyqep.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2jpbgbbsz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2deahggjc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmkawftd.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2oconlrhe.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2trwneedp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cnuvstjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rdqtrttf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wxksvysk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zstoqthd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pkymsaud.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ejkfiiyy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2jibbbnem.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2eyorgaql.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zpmtscnv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpvasna.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2bjprphyk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2axyfshuh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2edgodmud.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ieinkbao.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2uihujeax.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wsowxvmh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vkwsaimn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lpohzkqd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2njaoyqaw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2vzemvymq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dkboxbtr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pzjxtkep.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bhpbgsaq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2uxcoyife.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xyzypcin.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nplpumup.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gmnxcojg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wphaupwj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2psqiybob.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2azhscybc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2leuokpdl.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qjztberf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ioftqsan.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2abuizbbk.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2txhagcyx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pgbgdzyt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hwomwteb.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zsrrjsye.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkecbf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fzhpxcsx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jfdykcmw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bcywsodw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mvepezyx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxnybqw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pfsibcfa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tgrydxrt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2eqhzbfqo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wqyeofsk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jokpipew.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2fambkokb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ancjrexo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2srssjxro.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eqwgmnez.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2cbxcvhle.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2pudzmesi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eumdzmhs.html


<!-- 参考信息 -->