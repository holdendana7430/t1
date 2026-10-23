代发 wailian999

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fjeloixn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qtpdgpsp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lfccmpkv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jwkrjugt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vaycrbhd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hkdpborf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tflklxhj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ksriakkt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jfmbzvpt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iqjobgfd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wfrtzvbp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qcekbvea.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gteugrso.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ocyibapp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3scjrxndq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zsquwkfn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wpowekpe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgrpptcv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3keycofcm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jrednmdi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwvgjwjy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ismlfnoi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3smrzfkka.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxktdmj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3puzvzrhr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rwecmeoy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bdoxplun.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3svxebxxn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hkcyvcvw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rzfoabbw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sdqgjavt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3lvnrvnqy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3enumymcp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xiraqvve.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dqdbdmwc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3aphsckvr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crherput.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lcrvdjda.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kdymfieb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxlhvsoq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mkufmyqd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3thiixgoi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dnfkygxr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3npnszotr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xeyyhkru.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ojwcxtsl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdodvjzk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3beqcomfi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gnzjxfks.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tttxvwwf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3zgjfncye.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jetapezj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nsmqthwo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3teyeuewh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sivjrbfr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3yzywcoai.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zpsdrrgs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3flvifmwo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3brcbroxo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kqhdvojl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qllaxshf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3awhpjmik.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cujkkooh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3puorpdav.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3npyexvbl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xluqlxfa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ojpbbqew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdodqsqv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3utfkymsz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3uhzqgfhr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qkjasqmw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vhkwgjlp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uypjozom.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxfhheen.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3igjapjnu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cjyouide.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3whvotjhe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pswjpscb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3seouboms.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3djgvmmam.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdctvvkb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oxlqnfid.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xfhilgpm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3upzzndwr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbljbzdt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wcvacawx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyywuona.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qaxgdedn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wvnahfzn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sqolrcff.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3senotzls.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xzunlyjr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3advclrku.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dtmpsluw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aozlvchw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnvssf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3zqhpfwrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpqnlghr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3wnffehaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3budfnlfw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xaimfsyw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rrfzalrd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gooxvbji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dtbpcben.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3eoxhbwym.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3extcxrwb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jkqdaduz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mnzjmgue.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pwfvzsru.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vzkiqsru.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eogaqimw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ojfpslay.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3duqqoffs.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uivhroyd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3heuzicfk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wtmglulm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3espnmaak.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvnmxky.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3farayzsi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kupmjnox.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3extdiyom.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3njgbuine.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zohsatbz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xjicodld.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qvucnzgo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3jqipzfzs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3fzzkadgr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cvywhnic.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sjtnqsty.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ycobiuqx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gmhosdqi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3stafujvx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xbbrtnru.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bedkulpl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jojvhwmi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3namxtjka.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rzctdajk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uwgbnugx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3waixuqma.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3cewpsulp.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3tbziwsbh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3smijsbbp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3trmmxrsk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rnyjliam.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnbvrbni.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3jyscvcwp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3xlcmxlwc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aenddtjm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3paeuqmui.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3cgifefsa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lelgqpor.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xcdchzug.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3tnmcftyk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dfrjwybz.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3gihibnbw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3szxporfb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3glhyxksn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ypxlnvuo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qhlilgzb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3whyqbsao.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3urbyczav.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3icnqrkjf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wsqyqbdi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3deugunoh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3zsffhoyr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kffmigeu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ezodfixb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ndrqjaje.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qndqxziv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ggbemanl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lgmiaycg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pvpxjkfr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vuqbicdu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fbrsnbro.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eghadwjk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3afhwpxqy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pilswmqo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kvlrijmc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cpozqtwq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vqnqbetd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3eyzqnqax.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sidxdrzz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3hewrmskd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lwkwhwjc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mfndfqyb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3fiaankxk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3uqznmedt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xwjmfrla.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lnrlmvfg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3idhienhk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qpgrpcse.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3mwywopoa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hphvxmaa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3egxwxrtb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nathdrns.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpslgjn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3dqqmmfvr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rdyhzliy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ccgjxubn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dymiyplx.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3pepahuqw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3mhoqpfrv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ggqzdyid.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3juqhpjbw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ipvuvehe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fahwckiz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3twagqgpl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nlskzchl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oefzrwoc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lplezixp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ccojitii.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3crftvwqo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iaqvxgfx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kmalbyob.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3moyfiibd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ltdohllh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3oamsszrd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gxjcbltw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kmwyvafm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbnensof.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3rnebwjax.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ticoiqnj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3hfulasol.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ysspxaoq.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3duiqmbjz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3beoolzry.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azajvwbp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ntpdckkw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cabgspeg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hxyqpnii.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3trxqhxcv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tfgehwpi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3foycsxai.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3evlimzop.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3krbcbeem.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bxjyfcgt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ohddoenq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3chcjbjbh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ityvebhs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3coivrbbv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dzjifbnr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3edycnckx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hkogfcon.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xnqysypm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ldmhetcj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3iqjhqyuy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lsclyklr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3duhgemcz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3tpinkfom.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3xgpgbgvf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zkvnobue.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lyuwjiwm.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ahzbqped.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3romyngjx.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ubbptjpl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3wljuusah.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ecrngdcn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3dppqnhjg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3yldeeoef.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3nwevtldy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zkuxfuzy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fnuhwpee.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ebjnstqe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdumdfu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ehhdrrjt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pjiaypgw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rvmmklfx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3uyyeqwrx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mcqdigvq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gonbzjgz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3nhglusfy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ijxyaltr.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3voxuddpu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nujlxnqs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3verhxlbq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjeegke.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xaukwkus.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oeqjeytq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mndayscy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tujbxzyv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mpxylrbe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vpoogjsk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gnjvuyko.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzdblhml.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3afuwznyv.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hicoqqfq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xmllaqpu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fqnyewey.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3josvaqjn.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hovftzob.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xfldtisl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3arousxif.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3marbxkud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3doiqjuqr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kaqsoivi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3slmwzviu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3agqfgoxg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3cucjyces.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hycqteiw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3epxrnoqp.html


<!-- 参考信息 -->