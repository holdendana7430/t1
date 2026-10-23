代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yyhmhuyk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wktmhvpx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3assrwowm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pfucpmpj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zliklxvj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mylwppft.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3omxzkcvq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3wmjwhdhc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bvkzucnd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3unyvcxwb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dosivhlu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jnjamhnb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jbcwxdtn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbfkvul.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3elmygrri.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pejheoek.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gtlfbtdj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3czqtnphp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vyqzocez.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vfydxyxa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gxmufwat.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtfyjjbg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kxfrrzcp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nzechhod.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3crlspxmu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ttyemsva.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hrrnjint.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tnkgmucq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yherzdzy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3smuafjpc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gpazddld.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3amerzqdb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zumckcta.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oatxjodw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kazksbou.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jygxmlfm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3cvecoqnz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3enmxdfye.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ufjiuado.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bwzzobat.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3khqkgnrj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3jsoqdhvd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wlvavfej.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3stczxvhz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gybtnwru.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3grwamcme.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pltgivay.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eyvtvykr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cshzjllu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3byntuico.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lekjfzyo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ktydfjcj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hnmvsrbc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3crjcqjow.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3syojsecs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ffzfmxmn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ycsldssf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ylpxeiui.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wvivwyvz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3blfuwiht.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vpffvwhs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zfbjmeej.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ggqknzlp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3wwlxvqqo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3frchxeqj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3euapurxt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3plkwyuoe.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bphrgmla.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tkuvjlst.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tezgqwfp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fmufwzmk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3etorowrk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3enboxrdv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mvgpfwin.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oiqdmooq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3xspsfqmx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kkwbemhj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3weqmgqby.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ezaelhom.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvwuwunb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zvimdlld.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ojrrsokv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lqxvlakg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dkuugkjf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qefobcwf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phzdhtyf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3muzgaqjo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qmomprqi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3clwxewth.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qjefxnux.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3obqwfqcx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pduzheis.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3netlhfsc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iggyqoim.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jvjmchwa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pzztifir.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3spanpigl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3emltcduw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tuugqkpz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nozavnup.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gqxxlzhx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eozqzvpb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcbcmtx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3smdsvptz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sszyzkig.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kpbrwmne.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zdzuznhu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3otlqodnw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3byuvhizk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpgrmqfg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ggoohqiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3texvybkg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3veckxprc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dqugrhyz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mvevddlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3riuutnva.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ulgkekvj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3edgmyops.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wjupgvon.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3iwxthdck.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rovbhcue.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgmntkaq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3srmpqjaj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3nexawcoq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3efnuckfj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3znnzzdor.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dtcqkixh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jmwcgjkj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wwajncvj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kjpdbrmz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3vqbzdfep.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kayozgak.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qmilujib.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3njvpeiha.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gjxnuceu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kxnncjnx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vkfmlfst.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rywtjcso.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3crxqbjsb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pzvzutxo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3uwhjpbyu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zsrblrbs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ewgniiya.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cnxrgtcv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mdaxycxe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fjvwsiau.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3aqzrwrzc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sjuyqczs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rhjszmkr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3njtivzbl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oakzyuuo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xkyoyvfz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nkrjfjnc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tmygarlu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kxchuhpe.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3knavmbcn.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyasuyev.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3caavjxdg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mrjfumfn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtmphwi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mgmsgrzx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lbvqthcy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mkzycncp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pilvhjsv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ercblqpn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vgvbomdo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3icpttuqi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ksogapop.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pxhmrulj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3punxeyhv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xypieojf.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3lifcllet.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dklpauar.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jepzkpil.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3grvkttyp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ihcgnaxd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3varolfrq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sdwkduzi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3eefngwct.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vshkbdgw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3frrhignj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nktcioto.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xnzcevkg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3hmhnegzz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zvubuekb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hujbyusg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bfwbjzln.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3jqkntsuk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xnntvhgn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3koosnyiq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3gcwcpntc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3llxorzuf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3suuqepqy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mosoezxd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ebvckxtt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cweeyolh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cfdfeqym.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qujpsmxm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xkylitnx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kiwpibda.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zeojzdpa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mpwirdhd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3jqrosemj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3opnaxivn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3haehvknn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3feudeqoy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3gqkplhqq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbdotsru.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pjtxhgvi.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ikpgyyxy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3aufzzxdw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zfzvdpmb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3emjmluas.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cnskxdyv.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkklrdsh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3koyaroob.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dukmcsbl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3yeifuimt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rfqjpext.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xecsznga.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zfhghnyl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mxrykpac.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lttljsny.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3biaiudhb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dxyaebqm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ficjryfb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3imuikiwz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nezzodyh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3onpeeopo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yastdbvh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3zhnhmcfh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vepzvedf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vqkgdqtz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thjjfili.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbbqgmwm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3neztbltp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yfdvpbow.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3kiykypgr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3yhjhrzal.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3rlybgshc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cmmyjfsu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ugpqwalo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3amieswbc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lgjukrci.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ekwtxajf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3odxlzaxp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xcjppxcr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jcbkqvtt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iyoczgbg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tyijrrcu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vjzbjktk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wfkjdlhc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3epbllccl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3unpkfelh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kpuptwlc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xkarfaif.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3uuyquufc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhnxrdb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gamusqsp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3mgfpvkwp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ugbcfglc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3vnjgzxqs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3orttkjne.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hwjtybmh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3eenmldqs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qpzeymsf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jzqlessm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3neunvsdw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3avlyeywm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gspsuxyg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bdecunql.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3glaweyfx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3tvcusbpq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mvsgxijj.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rsipendr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lbjlpduu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ddjqrkni.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xrffuwff.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eoktnguc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pzacalos.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3olgemefm.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3skehrqdb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3llfgliek.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3gwzjljwe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ndbemupg.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jkqmerph.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zgirxcrm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtlcycs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3itxexhun.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ephhfjku.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hievfuhb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpklyxn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pcpqkpzx.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cchdbjvs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yhohlins.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hlhruuwg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijogpyuw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3aximrqnk.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nzgumbyl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qufnrbif.html


<!-- 参考信息 -->