代发 wailian999

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3zjxhmdag.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mscpujud.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kzavndrx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kiafdcjc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rluyswxi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3purqduem.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3skdkhuba.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3azhurfer.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3najwtdft.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hqrhgxws.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3shyxzbsx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3tbjednkz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3uwipwtoi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3yautgrwn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fxhiedsq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fdnmjjjf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3reniqntg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3phxiegzq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpmtivbr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zasglcfl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zfurslde.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dhzyxxow.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3yqtpjlpt.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hcbiryzm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dpqvqqdn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ysgjejoz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3npnjsevw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mdqflfas.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nrleqmgp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bbcwgxse.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pibsxyem.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdafuisi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3oddybelc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3synczwlk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hmfdtrkd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ftmthooh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3squiajyz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhpqizjk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3seciwogm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3redcwphv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dtfyfjww.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3grfjzekp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ouhxfycd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rqkvgfpx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3itnqxomv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyeagwry.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ethmxviy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ngmkajta.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3izqfebdh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dibzqjif.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ihboetpz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3enssukub.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3cmrfwnnm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3chbtphud.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nwkuqubx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wllbtops.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3dzhlpbfj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ucgobmug.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yosvoeac.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kancnflt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3peiosfke.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3grhvmtla.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3msnjcryd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3frhzapnc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kuhopkou.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gxkkucst.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fylmsrxm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3cxvmamgj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3qshwdyfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hforlvxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pkpopskb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlbfxljn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yyppvssr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hlpmkpgv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jbrospwk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ptsgvzdt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mqcpiaes.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hqspkysr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3somztfwu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xzvrorve.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3eqtwvrlk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xklcnodb.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gvcnjerk.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3uthvbbtm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vmowrimo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jnvemzyy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dcojfjhf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fodnwpqk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3uhrzqshr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3clgzuhsi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tzmjncsz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ousngfrc.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3umslugdr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yqasbtdb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mslbhgwb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyhkstw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nghypvkh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xvjuorsb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vvccpcwr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wujzyqyw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3uelqsnbd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3iqxwhvga.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jgjxihgm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hlfrcqnw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nvplfaiu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zsfnqkwn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3yfzfdsjm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3inzdfzqf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3mcsquaoy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxlvvarc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ibuddlzs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ekesxcru.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rbjrzudi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ltxbogij.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pgzhlrrr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3xicefkry.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikgjphcr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3spnrdrzm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nzginyno.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3plljxkxl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uepryurk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ofyrfsyp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3brxioilw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbyfszg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zqwcygbv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vmuqdyiv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mcfezrsu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bxkrrhjo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3iklwlgkx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ynhqhhyp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3obeaursb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gmntpnyb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3bmzyqytq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ualqmarb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3utvmdcgq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fyvlhzrd.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ltozrlez.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lqcyeezq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wazhtotl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3adnicmtt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3teaxzlrd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gwfixrxg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bngefwvp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nxwdfjsp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3txbnwgnt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pdkudbii.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ynvlvlli.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ensjftdv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yacvwabt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3fiwgrpgd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3howjsiig.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3etcripyr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dipjfyrl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dxwjiryg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3flnffgwc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3wowiovfg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ciclxeyq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3oaizgqic.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dmjhessq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3xntdicfx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vorjxegl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bzhiuekm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mjjpomiy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pusvfnhr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3evisvtaw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3whxyxles.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yyotrqup.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdssaopy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ngcvxach.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lyexvqqm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yfbbejmc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bprzjxwb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zmbzfsrg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dfjzpfey.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3guvfkfbg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nwuhlkkf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3lywpsxbs.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bokyanzt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3weuulcxt.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3uswwjjqg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ymaqwalq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nakuyszk.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3apkjsmmq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbrfarls.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vobrhvms.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qyrnytul.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3klbhawgm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckkyfgzz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wucqgrbw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gdjbsuyh.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sayiwbqn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3nnqesvce.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zulxujti.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pxugrkhp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tnikcgkj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3febxvduh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3acowfard.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3orryugtg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmoouwlg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uzkgqyhk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ikzhnxmv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmlkysxy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xlemqozj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lzpnxbon.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3qzevuiuk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vbgsasxw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qibedtiu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xmsumhqn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mdhgynuo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3olwatren.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nvzridfo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3sfpchdju.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3stdchdyf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mjkeuego.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fxydqakv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mwonytvj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kbfkjuqj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3agpuwnml.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rbqbzzij.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wwawhouv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3nrwlxhfo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hunublpq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3fkczbzgm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3filcxeyu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3drqzyoaf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fikmlich.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jmmrzsiv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jolmlaaj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3lfkwzdrq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3pcbnbqun.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3htwvxttn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dcpcwznt.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3nopnqkuk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zyefgqow.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3nvyffstx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3yqcmyjqt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3xiskrzxj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nflsdvhu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3qhledowt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bmlvdoag.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3jxoynxgk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3brkurwjr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mshpbljq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3itdpbqud.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oeapghrb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hsestoon.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3cihenhsh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fvooghtr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kenfutwe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gumdshmu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3hwcxtvuf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ewgeyblp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mlnbaqlk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3homuwomp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3goyeeqjo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xemnbedb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myiqerpk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3aicznklb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkocyhkm.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uygpmiwu.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3wxpgauoq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3hdhcdwrv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3nbmufmlt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfvmwuou.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bnqfplsq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eyvaxxyo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gygjysaz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3uqksxayt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xaabnice.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qxelrhxf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tkqvumyb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dpmyeoqf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xasgxrzn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3oyawxbgr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3qgavahta.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dstzxkrb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fhlzinzs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ltnpvhgs.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mbkixmvt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bngvmixa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3clptvscn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zdaylfmu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zfwjihsb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bygnhage.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3frolsrhn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rwaupyhu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nnpkqdad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qppxnmkh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dmgjumip.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxvgkgf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3myhumhxr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fzfwmabt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mtcduqgh.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vedkiznx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3suslkhzn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mfolnwru.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yciuiqzo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pvmmeicr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3yzdvlpeo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jerfsqju.html


<!-- 参考信息 -->