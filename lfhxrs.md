代发 wailian999

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3inmirsah.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ytguqntn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lwhrjnah.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sduhleot.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3trcpoyag.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3arsvcore.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pdmndlxg.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gtzahpyl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3limdujyt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3mmbgppac.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yhowodbe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zobdcpng.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3aocavevu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xqddklgt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwyvayzk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3arkfjwgx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3btxwdnqf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wrjjsjrj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mbnougvc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3mvalgndb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mhqpnwvr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3kzftxvvq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zqvzpvop.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nxkmdyvr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zokpywjz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gdduqchb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jojlacxn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fxdavbqy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jyqpuihc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3oytikhkw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3yiqwdvwk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvylokjg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ekbbljqo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjzeotq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bftxxtsr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkymraas.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3revzfhmg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3agyoanfs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3scrtsevg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3aknftvdv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qpvorwan.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhxqsqsk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bstlyfky.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dpvdijtk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mrlemgqf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqatbcwc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yjhmihmp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fbwgmtvp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3swwqthvx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3novchtds.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ntexafie.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dprpaslb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3waxdnzmd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ddcnapkg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3juinheuw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hqfcfobn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3isvcdbbq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qnnwyuga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gucrunkn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ffmjhtkc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fiuqfnww.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ofjfwaim.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vstddkns.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xszcobxj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zvrnepfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlgxbhsl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uierkzgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffsebfry.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jsabwtro.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3muhejcoh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xixorriw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3okmqqkex.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3cegshztm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3owalwtmu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ezlmxctl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3gncbihes.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cqittxkm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbtybcep.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yjaelteo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hdhhxlcf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qxkmbjbp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fewxjddf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vwamjhea.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ogdscizk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bivwqkcq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3hrxzztvi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lmxlhlkf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xpdrddln.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yfyvwetv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiikbxfc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3thxlvdla.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3baykvfgg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncxfozja.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fsucjruy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jhyyejhx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vvqccyii.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3drvponbc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dtvzstdq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qatnyjee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3drnqjati.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xhxfrxjn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3thjhafza.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fenotrka.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmqgel.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kotnrcli.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzlvqum.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3eoiesovh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3vjjbrzel.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ioiwkhsb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gfigazhz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3offwnnlf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jsllwkec.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3plvzxgzb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3imjmflxf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3naesmogt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hdglfhwr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zfhkmmmr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vcvasvlk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rammntuv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3rxqfklms.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cavammdq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wgzyklag.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rstvqhfe.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mnoiacst.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3grjchcsf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gtdlieoc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rjuxjuhv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3veqyjjqm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xudliuhe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3boawolhx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kfvlelra.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ejycrfut.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lylqsszf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3slpwpygr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3apnsgkvl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3twivajgz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yoxyxdpk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ejcoktnq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xhyjvxfg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gqmqxerx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3zbmltefk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zqmndtsu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tclocozw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dxmwgiye.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yoiaegxt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3flvbjniv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3hrjmdagr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kaprpmfz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ldxqgmit.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3unhmxoqy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zhhoczkx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhusubf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3nptrxjtm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yqdlfgnt.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzawyhwa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3hdzpbfkx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wzrwarwp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dabwylkz.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3saumuana.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fwhklomw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgssmoqy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3lxrvxuqq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swmeebxx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3loljxoxo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3acetxhus.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vubufjet.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fuincvyv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3leubhiix.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kougimhj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qaksrtad.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3sxmvgkop.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xnyrphmn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3hoheznow.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xfxzxsnk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3txrbbgcu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zogfauta.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xqvdkfoj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xocangwf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bcpbrgnp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugtmegjw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gxybihen.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qfeazniz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ywmgyrkb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gfuyhnhi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3hkutwckl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qelbhwgr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3tbtgpjzz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ezqptrdm.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3xpywpylk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddamqjza.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ayevkgwb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3crvfxqlh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jooyjdnt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lykldwsb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3lwfwkglb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vdzdwfad.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jvigtlls.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gfohzbxh.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tlrahokr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qqofcdpz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ehldadbe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3avaeusmx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxyoodoq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vabfynpw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3irkksvre.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubsxpgev.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yavoiihq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rorjyxnk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3abzcsddr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uyeukebp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3jkfsnwnv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3uxacgoug.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gligbrht.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3quaottog.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dtzhbmaf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zshejflu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3guodjyqo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wkgvsvnu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3smjuiujq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qucbajbu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3srbsclrw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3nzpqnnxb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jtqygopf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bdmzgipy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3fteufqyh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vglqaitj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qcwyohtc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dnyrjgur.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dnqexnyi.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3vguuwdaz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kwrozyii.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xauyibww.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3zhumzqky.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3morhtftx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zdifjrsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ciywkfpr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dyhjvxvd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zqdgrdni.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ytrvjuac.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hdzltakh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3umvtmids.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fxgynbuu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3rqztdtzh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlynnbt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xxqljceh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fggiegof.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wdinmvzm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nemwilxu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3uxpvlzps.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oddzwnff.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xqgtjirb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qkasnfjd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqvxeepz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mzejhcip.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3owbevjyv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3knlcsmqh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3vqhukrni.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jgreogul.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3godhamip.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3czxsskjo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3buxdmnpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sakwzfap.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zpjmsagu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3knpgqryc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kzfzcdas.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3uxusxhww.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3xusnxyac.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3btlfebys.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pamdznpl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqmcvfi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zzqrcgqc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tbvvxyxo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tmfqctyo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bryozupn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3smwlgoar.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xacudvvi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tawhbxsl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dnvkbvnf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mgjepscb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ypgyezjv.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wbjnpqwq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qdvzxdec.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3txsrtgzu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kdszvwda.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xupzgjdu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dslaofyz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kxfqtchg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jipfddld.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3btsoigav.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ugtuhhgo.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ajjbqybs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kghroeha.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3biphzwcq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tjxrkxua.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qmsqauof.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uyuftmty.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3augbvcem.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uqmmulsc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jgrturdu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbtmncjp.html


<!-- 参考信息 -->