代发 wailian999

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3prqwkags.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tpaorism.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3phlaryhx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iwdunqpt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vqpcfsol.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wlzewejo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dggvdcow.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kehdjngb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aghjznzb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hsgaqznb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mhrpwock.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kqikifzo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3znhtoqgt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3egwsokej.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmrnuufo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3swwfxoqz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cxmorzpd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cvnbrnkx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fdbqjlyq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ugsigafx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iyegeelx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3erndhnmw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nngmqhsn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bamqbaxw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fbsxvgcr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3aufkgdym.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3orxlempw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fhazzgdc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ytimjbay.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xaxsmgdg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ctwnzzcs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oahezrvk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nscmotgy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rbkbbpyh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3oqvktirq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ttorvzgy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3whuzkbnk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdszeams.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3qksqdigz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jrrytsca.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pcqhgpbn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3augsnkev.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lokcqygh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gnkagjkw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aguehzpq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vmluuvnn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dggwdjfc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lnepskme.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wrxznyzw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ejpjiice.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hmrgxxcv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mjgwryii.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3uwcepnyp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihtdsets.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqvbvtoq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dnvlvtrm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jdzjxiex.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3inmnjmxg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qkwtwsxn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sisinaiz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cudznwbx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vvmfmdrn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sukobkfk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bhbclyas.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zyhlgxyd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3orxaimvd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxtrmxqz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gvjniwxr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3knzqxujs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rsuujnuz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tuigmoih.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upabxcba.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bsjywznx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvmrmhhe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wfthchpa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3abydazhg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kxwfbmre.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdavkhxq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qtfsgpdm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cbuqodbs.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lhatjokf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gknckhsi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oacpoida.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wyhnkaze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bzkwvigf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xxkrhccp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3omczlucf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3swlqardv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tlmzvryx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iyftyiqs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3owdfjoar.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hvjumhjs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3brdnstof.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kipzpzct.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lotvmbzh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3utnoclks.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gybletey.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rocehsgv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3eksnuzsu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gnxghinb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bpydamhn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3acyuqunl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3erbrkuff.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3njjahazz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qicfdxzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aciieyoc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eccdaksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdwetjyy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3znayngju.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xlbrvyfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3uleshsss.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lkuzzjck.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3aeikmuzi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3dazwohxt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wiryxyte.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jputkbyy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rfzcfgti.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gwzdhnus.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uxbyomkj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wvxzbbxu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lrkubjbu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nvzmhmzl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3yqlshgyc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3marjrroc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3glgsydqm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ssvatiyp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cqkocyvv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yinbuaxj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yarbcjeu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwgcyxbn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jsnmzxnm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3keshzhof.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nzlasibn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ebynjruq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqnorhkm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3riswbswq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3meakcmfk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3edytiwsx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vjoljorz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3alznushu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ayigwbxg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3aboinhtb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qkicwrtj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qtgthcco.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3stxojlpd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bpxdnjai.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hnwqeppo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3efwvkljf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3myrulzbw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hvvdjbey.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3txbuheip.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tdjalqir.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzpchadd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qmhdxasm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vwkbxhix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zdgecjuh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ttxlhcbf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ooghfslu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xtcjhros.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3alyhojbk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jahxualm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lrkpweww.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3tqcsagcp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3sfxqnyxq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bijbbemk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3lncaxfhu.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mtlkmwgu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njmlztrj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pdhcrtcv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ulpuxpgf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tywgvwtx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3dgmjoszl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3eqewcrou.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3urkxjhbm.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3klflycpr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qpbabwnx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dtmhbqdb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ghubqynv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rpionlsx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vjuikhcr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yyvacdos.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3capwjloa.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tneygryr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3gjcyleve.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wmyuavjc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3erocyqgc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3akqrdbew.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hxhyuqmq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lnulvpuq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mlxykwvi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3epbiwccd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dchbjzpi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jvqzscwu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pcpcqoes.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3soahvypw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pnoynkvt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3djiwjkaf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pitbafsm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3iyczynub.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zdwypike.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ansrxpyk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3eakvdgrc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ssitaxlb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hfvebedd.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3acrusmcx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kzyszyeh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3hqmalzlw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cvnwgnyi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3mrnfdgya.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3lssreush.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ctrjftaf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ggqsrdkq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nsrmpiwv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3idgbsmbn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3bqadttmo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3vpanyvff.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3uoipdwhm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ynisqrwr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3aghyoedk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdknofd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3efxxedcb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3alwyjyer.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qxfapdlp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3setojezp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ttoikrvk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yzwxhkkj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kxztlwor.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fzflcluj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hhmoclqz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tamzhiim.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3eacupbcm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lxmqukqf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ghaxgqun.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3bjmnxmeh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewodcuie.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lqayvsps.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3vakmjuvz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ylwfxunw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3saiqqyce.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcykhzp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tsmrfnru.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xdcbohra.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3wrgizwym.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kmwxohxy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ftneoexn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3mvsodpkw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3pfqpddpd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3rqqifyfl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rmkqutcj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yjxqrhfj.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3yxgktcry.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tkkuigef.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fgdlfmjw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rveelxeg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kdmjglex.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vawwtyad.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gxjgcbya.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xwumhufo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rkwrevvf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3csqkfozn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3psynajxw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3akaibeug.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xbkitrvl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tvnqixcb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kboiokfe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ghmayofx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3tnwpxfsr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lnaoosyb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gbqqbmtl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3hveyraar.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gvghyoax.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qsiuuxhx.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hayaeefm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3poefqbmy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3asvyecah.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ntjvowll.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lqwcuqfx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qjykybqo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzchur.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yvogbxvs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ahaygfqe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zegmjixm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ccdulrfu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3obxhuvmq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nypagrzh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eiaasyty.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fuhjlqcu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgvxobb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ybgrdazh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3oavrnbcy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zvxstqzy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3upbmbola.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pyziubah.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vunuqcvm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ljjkegcj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nlfmczxh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jnfmhcsz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dyqszzfn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tjbrdvzt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vepooyun.html


<!-- 参考信息 -->