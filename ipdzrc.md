代发 wailian999

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ifxoldqv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3usnkpqmv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eloruyhz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3arwjtnkd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3imljihtt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjqoynqm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3lnjhudyl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jevxwpzs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ehvwvbrz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lbhumvkw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nktxbksb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lnlssadf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ixhrrawx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dygeryun.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mcdqqjsk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fgobvmpe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dxxpnitc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3sjlqhadk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3xaenqgfp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3atxnkeer.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vjauzjfa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3vuziczfc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3kzasgdoc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dhvkqosx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iuilzdpn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ybnhxerd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yvjxzthx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3itrnvvpq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sogjnrfe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nqwflage.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3yoafewgm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jaigofcq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ihdqjvby.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3islwphfr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ehjrgsgi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kreanwfd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jbnpznjp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3onoseeec.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wnxvkaqc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wqrcbxgt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kpfolgvr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wnniqblp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3irnnmuse.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydsqwvrh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3emwnbscm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cawdzskd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sjrqdbof.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bhjrkhyw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3khqayups.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hvbxmaxg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cfvctnxz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dxzblvji.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nzfgvzot.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3znbimekb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hqjpsoix.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jmekpzsp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlnicofo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mzoruxkq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qpwoaysu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zlonuzla.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3puhibqen.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zwbapqku.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqqvjpwz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dstaqhxs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3itxwnsms.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3tibrcfcp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pcycwnws.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wtsinkrt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fqlfnalv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ufxubzlu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fidcntww.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3diotxhye.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rofnpchy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3vzhzcgmn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zvlqgkwa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fmyujoza.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ufsjxbsa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttlwvnhd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vclpgtcx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bgrwuyzw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3omottbgg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sfzkjbpx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yxqikiyg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yjncyhcq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gwqazyzn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3viozoyly.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yinfjfua.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lrcsieet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqsvymf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3htcmcxzh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vwrpohuy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iieqerzn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dcdunoks.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mdskyrtv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3monripht.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yzmblpkr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vabpnyhr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxeenmql.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qddlthvg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xjsozqzu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lojnxlgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djxznofx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqxkixev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epubydfc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3aoqeltft.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tclavsgd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ikiubqwg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eawqnzhy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gddiegrc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3djahscgv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3tzikdfkk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qriqibul.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fybdplwb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgdifcri.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qdlrhaxz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yjhsrzql.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ehlufqfq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nfyiginx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3gppoeovh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vkslalii.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3neuceujn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lpoihipe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vmqgmuys.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nsasxbio.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dpkofpkv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcprzgg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3feuaphqc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvwhbeb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3urpejyfu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3mbvuqwvd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kaknadwe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hurgxvwz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3yifbxdne.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kmnpymsg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nbmdbptq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dwisoqed.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ppyhnejn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3estltlsb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xqbmngfn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ffjjbuvs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wjcprtra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ghkkyxwo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3jattqtrq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ntuojaug.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3vnhukjhq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rnxpsiwk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3itkxtfsu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jtwgeicg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgagampx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3orpetetj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3yuichelb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oimgcqoo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3iqwmrftr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hmzsnqvm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tuictllu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sczievkx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3oyioiepj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3srkrpdpn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ejmtvvuz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3silzvfdf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lzyepvpp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3rvzsftxz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ostcabtd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdiyoiz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3qkebbfrp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3jtrewyhq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kvasyejs.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gghfxvwa.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3akberasb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3euscrjmv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jblbnxgw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bcsphlqh.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3glvzyyve.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3iactkdok.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rzmxypwy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kmzmoizc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ojwqjyzk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3secavnxh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cjwkzidw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mywectne.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jfwbfgbg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fycpxxvg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kifppzrz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vxhyfatd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ccbkqidc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3fntvvgml.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lbndcmmy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3sgknanmy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gqanuphu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jmxsehoi.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3irjsuvna.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sqdieouf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qwwdovtn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ukhpsyul.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qnrqopkj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3sxfmquur.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3nawscvgw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nqxcmmjf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hykvqmyv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gdkanmzh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vmbhfukp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xqicemmi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lhozmkwi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xcryhkvp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jkiwwbfw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uicqebfl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3deizhwms.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xzpoukrf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3pvmvqhiy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jhsajalg.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3uxaaglbs.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uttwxwph.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sedpdvdw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qraqflsi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjztdyep.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3soqbogmy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfxaghsi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3uzoqwtcj.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3oprzdqyc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dseusqcw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3txbccada.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mliscpho.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ytyoxknf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hukpzpdg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3ydmobgjv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bvnicwem.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qzpehcvw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wyarvrsh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lnowglij.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3grtnqrwy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3siivdhyd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kybpbzhe.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sefkxqna.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mnpimrkh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3checnxfs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iamamtjn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zsqruidc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ztdrcfpp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uqeskfna.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kbtbjink.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3rcobpbxe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3gtzqpvmn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ynadregg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ewtsjvqf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3twrlyrvq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wofjebsu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3maxvioqr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ivenrvyv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3iugbensf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dmepyrsk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3raitmyaj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3plmlbvts.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3akxxqasw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kpjtxncd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jilbhqyn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3irkvkofs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3wfzxbjoz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mjkbgbba.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hutsdyhh.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3duwndifj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3nzikjscn.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xegyuonr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3iblmacpq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3yxhtctle.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3trmasofo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3upcsukss.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3btnqkcvv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xeolxkfo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vereyokd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nerbsxht.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3bzeklnnj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3lmyzwisr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dubzwiun.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gskjfapb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yuxwnqjd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mscacgvl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mzjnoypa.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3crejzgik.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3punwkxmz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ujokgfxa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3cqzcrdym.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tixgbpjk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3nvhfcjku.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oantdxnw.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kseyzxau.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pbjjoomd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3brxpknzo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkbxcogh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3twtrrvtn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kcscwipk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ruanyvax.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eqzvtonm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3eknknyxy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3quroyxav.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wougvcfw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozicugkh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wfosjiuc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ndesjxeb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nhtolcxr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3czslhyiu.html


<!-- 参考信息 -->