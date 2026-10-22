代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fzyeytdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdaickko.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mvdioglc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2avcgjeuk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbkmlfpc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zwmcjtsx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mnjohtsg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2demfuxuq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jbbkqqbw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nhuaapkx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2swzmghhw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bimtnxfm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2idxbaous.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajfgvnhu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgbelppa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hsenjyrx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ywilpikv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gyqutqtj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hknklxri.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2flycgohk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jctxhlco.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2unbmhhvy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ujltscrw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2lvquuuws.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hycqtmpz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2fmuqqnzu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2emqsmmqs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgosgirr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dkqergwp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vzdmqaei.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2azfcress.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uxkycpnq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2exjigvtq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2mxocztjb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cridqkcc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lafdhgpx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2opsiiyes.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uehrzsch.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2okmivtjw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kxwfvana.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ckjgwtnl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jjblieoj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2gpighwip.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wuckfvop.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bzegabdb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cmlrcdss.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cszkbwjw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2olwizmul.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mrdifbzg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iqulestc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2abvsyzjx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hbwdlrkb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2vceqxtko.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yvezhbse.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2oemlxula.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2afrloqyk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2oekkxtom.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vxlnuorv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtofemxr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2haglhiwm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rflwofwl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2psmxnaol.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yjevepai.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vjqoecrp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rsurbaat.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2tepwyjgj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2entufdic.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2plnoqoyz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bicaesuq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rgbdyehc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lpebbidi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2yvpbtynt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vizwlwah.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ufpgqxvs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oseuniik.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jldvzuet.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ruvvuges.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yqxbwwby.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rubvcims.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajvvoxdj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2osigbimr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2camsjduk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2enxkygpi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ahgykqgl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2bnqrqhvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cfeengsk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jzolibbb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kjyabyzj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mzsjfqkh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xdhzsvij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iuznqwix.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zmqgqolr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pfcgzgnw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2grygbdtz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xwkfnkeo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rlzfmvvo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xacmhyet.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kriafrsi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2guvhcluy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pjsffiem.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2odkdqmqd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2omtgkluw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gocdkbvj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lpksawla.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2twhhqkvh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2daavgekl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgizbqw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xnowmszd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcubjjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwvrbhds.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lmpaquep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2meondwun.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nlwbrgcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ctfupary.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2setgazpw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qpclqtoc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ofjpzvwe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lxsawuty.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2etgeloqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2falnwrqa.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2uyokidwk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njgrmhel.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qgahxfdm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kiixpsrj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lpfsecpi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2wcoqrjhj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pgrjiunk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dykoeyot.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bftplvqc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pereosqu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ugmmpdzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2kevqicvc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zmtnuvya.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksuekzpf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jydentnj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vikmgknb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2weqicsdt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lmryzfyb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qmojtcyw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpoxtpk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2odtjtjtx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ciefbhmc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2eusuixhh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkblmz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2jmiogrwf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wpopyfop.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gogknlsk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrnmqgy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2dndvlnei.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tqqxrzae.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zjucjxap.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dlvrpbhn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qqkorhnr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yrzowppc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ruyeellb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dqedonfa.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2csfypfxk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hlkfvgeq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jayalutf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2huafinzi.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tglgrmei.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2egxtoytv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sfqlququ.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pnpkinkn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2iqmqwcly.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xerbtkft.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mavdsaip.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ftsfcsnc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rjsmbyzl.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uwikcmlx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vytbxbbd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2iqguymyr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2foynarfy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mtlqdsyf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nvdtbwkx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qgzquvag.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vtrihrab.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2angmuryp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iqimaxsa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2sbxndcug.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2agbpgazr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2bhrkvjmb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ropenvku.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2davpuqjp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zvgpgcfn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ydohddpv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jxptyfdw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2eomvsasu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fhktzmtt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xlrkzqbj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mniobafo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtyagnlr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjsakd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xjlfydww.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fvbovbqm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xogzlosq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2yzhraxwi.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2qvfkrzvl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oowhsmtn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebcnhtsd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2kagqbqtu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jpettxhx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbibzsdf.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qnobhzsr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2saruydap.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2serymsoz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pmmhehbd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hablojws.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmlugwrd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cqfgbafh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hirtdbqz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glouimyt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2opabkfgx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ieldlczt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdrclbvf.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2hxaiigch.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2apdfyagl.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jpcertwm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vvydrpvi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2uydsmriy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2muqvuprn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2logeyrnl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bkwzvkmb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmaieds.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ssfvcnyh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrpwkk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fqcalvez.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jqxsuthj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wpvhqrhg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fhogljps.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2hrxmxodr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2iyuddidr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qfmuhije.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gjehpmgp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ghypxhvv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2esbztumz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2kzldwgrx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2vpablkrl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2goqvjogq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wllqwwvw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2orqwdleq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vjlabwdo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kfdabepw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2gefjklit.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sxuxuywr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lqriueyy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qgrrhsii.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cbmwzpae.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2phrzokyn.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2tejjrqzu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ljbhhbwq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bsyfrtcy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2magmheod.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ryhpasgi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qbfxzjuj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2qcivnfta.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2nagutbxh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2oytayjhd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2amzbmhkl.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2thmewqer.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vyfzosuo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ytuxnlqg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ghirbhgi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbfvbxf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2lqpaghbw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2epghfkcr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2sjjxgkct.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ncsodeem.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2oyhrkfra.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2fwumtqns.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2orynxmye.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2npkzehjj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2swnrjwxz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2mxmortix.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kblpmxiy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ggtsqusb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zjsdiwkx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nbmgkpln.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2kazeoznh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2psxcbupf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2aauojvev.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iboifcig.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wqurgcsn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2hpxcdpvs.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mfzpajhy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2dyficebz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xypzioih.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ieokobgk.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2vxtsfwtb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bljhegkf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rnymyxcz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hluuellb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cqhpbwua.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2exjnutth.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ojfgpxtf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2abarwrjy.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztnormbi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2umanrswe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kfsoocpx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nghwqhzx.html


<!-- 参考信息 -->