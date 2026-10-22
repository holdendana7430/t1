代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aivkyuig.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkekgcla.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uzulnscs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ocseodkx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bivcezrb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ngnchqsz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2woymhecb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ybeehpgf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2scimsvmg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uyzbahsn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rpofonwp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jgdfqejk.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2csamyxdb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rdrkxlrw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iapihift.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2smulhros.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ltywaiva.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kbzmwxsd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2siprcaxd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qcjsnrcr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jzwyqopi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qlwvylja.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bqifkryk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2iixkvyiz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2eeqcsqtz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jjttzhaf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zoesvwgf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qetclkvt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hluettoo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2efveulxs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ixtfottt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dgkhdber.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mvlzbzbv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lsuymdql.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zubjhrku.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhaqyzfn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2inrkxjqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2syfbrtcz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cblqelnr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlebeho.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hjkkhfgb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qaxapphg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bsotykgc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlemvvd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fzqpoxun.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rrgqyvjg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mambzzks.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ctokqira.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qykwpech.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xcgnqdux.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ydywxwmw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wuziypuw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vjctkfvq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kztwyimv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tnwamise.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bsvajysw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pskkmebe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rbvpntjj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fzvxjtaj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bjeautfv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bjlxzmwh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pwghjckk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbymkodn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2brepktmj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pfqygavl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yntzugof.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fvjpkvsr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2enyfgcpd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ggeatonf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ylqmffgi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tcvpntnl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zesshmkn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgyfmnll.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rhdoywvp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hefzpkue.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ogsknjpk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xqqycewc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnzkprs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xwsipwyj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbbrorll.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2itprsoml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mbajbwoc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oqzpxzxi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2sntocvaz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kbfrnhmj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmyjjfzi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ouhhvssl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2egxawlsi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsnfqhre.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddyxylev.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2njozzgll.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdhqommx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cscebveb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rdioxvtt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uzbchnwy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ebkkpfvj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gupfxjev.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rptgdjer.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tvgyhmpu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ydvthtuh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fpkasgtz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eonteznb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxjxzlo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zelpsurk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lcwienzv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uegqxpjj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2epdckmrh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ndcvwiuw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rhufglsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvdgkzfh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zpvjbfeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ambujdzc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fojucguv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iashgrdo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2amvphfoy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pezzpfgl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sbgfavhu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2duodbvdu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2irpsghvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jyijnlwz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2euyxuzac.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ekfuswwz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jhoysygv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cywsgijf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jegzdomm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2asfalcvt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pwqwoyuf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ccmwpjle.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ngotaied.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qckwsshy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2izyxsfjv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2faogxixm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yufzdgpv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgynavg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dwcxjluj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npqjepdv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2iuvjtcwo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zgbkujay.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cbazhbvg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cwsdicca.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gwcqzgrp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2oazkoamz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ikxfnnwy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dznjsusq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xvdjvfhn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2tvtrjqwj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mcdnkwqp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2edngyabn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zaaktyty.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2oeowwohn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xrkielkb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ibotrptj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hqpywjia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eynmtkbk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rhtokjnl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2dibeicpp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2iujzptbi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wzovlwuk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2taeeclsn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eedrncpi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2btbepclw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xzajlnvq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lbocfnlx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ozhrtmvn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2lnfsbdvd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tkayyhak.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ewusjcdg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gqjznvhy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2euattowj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2khhrlyso.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2dyzlrkow.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pyvtbchc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2borukizp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nyhujfko.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2qmwszqie.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dftsddjd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2dpoutvbt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2yyxysema.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oprfrhnr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2awpzvocd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fogygdbe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfkkbdn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qdmmeflk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ukupsemz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xjepqdsx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wsdlghdk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cjbnqvmt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2hhjvmkan.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2yltglpjy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qtaqpzfd.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ajnnoguc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ihlmesni.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cbqzdqfr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ievqjxyg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2cbqllldy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2aqwsvmlh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2udszqvmr.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mhqialsh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rtmrjmbb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebwkyfko.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ztpnagaa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vamlchyf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hkqkmzlz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2nubkpbmy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ccgmahfe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2uawauyrt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2jgxmffxp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zpipitoi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xdlhbfhz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dbqjhpzp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2mafbsfxi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvdwklro.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2mjgmmyvg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ebwlwwjo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfwclwuv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ezhxzimn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cymkrpsn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2weinysgu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bpyalnbt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vfqxlapg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ycveuypz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2keatbifc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2otxuemiu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqiqvrrb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pkrgbjie.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kokshzzx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tcffvdkp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qwkmbvda.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2omanridx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nvaikeam.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2xrtjckoq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bhaazjzd.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ftqpymrq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cyzpputt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2evllpzqs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ruhhmddp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2pnvrbihy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2injffwuz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hjlxuaas.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2epjaqkmk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ejekjjhu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2idwtulgp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2upwkpzbw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dfmdwfwb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tctguxhy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2niusfjdx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2sebxkkph.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2olrgtgbj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bfwnqhtr.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qwgevpmg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xvnvyczv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ecfqnljo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jqyedthi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rpzczmvb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xxqbdmud.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ewbbgzou.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bytzhcmp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2akvdjvsj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqkwfiqs.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2sbhhirlv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tzmaeaqb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nswrdctb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2emxzoyfp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2knqyfpfh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2rgcivwrl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2rubhwrto.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qqfyaekl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2dranzhmf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2cbyektfs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jqejevij.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ryybbwcw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ybsbesoj.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cnmtyaze.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vtlpvclw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2lcatcetm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lhpuxggb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qwfxetuk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wclnqmdv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2vhjgcfdg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zsswsulp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zzcfvbgz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bkjkdjjy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vhajmnes.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wbenpfcy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2khojssff.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2uulubbvz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ffhrlfhp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2jmokyepi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nkkyanfz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2abzbzctq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2myynphvu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2enbvywfn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mkdxsczf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2eakfznef.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jypmgcvz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2csxkpaxk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2unmwxkxv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gdzikgew.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ukxzjrjf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yoyntjlw.html


<!-- 参考信息 -->