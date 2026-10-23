代发 wailian999

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lhbkpqwd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fjvduyvg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zwfeugpo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3izxsjxkv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3hsxlzitw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ajaskfzd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qllqyusa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zaxwnzhm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nqklplru.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3cewnnikz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3nlopzvca.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eyengnud.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cvccihuf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dlvqhwse.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jgpbnjsd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jzambtmn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gnmvctna.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nbygjdjw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nkittmri.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yguxyffw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vpfvkwox.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ykmubwln.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ntgugzpb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oipbmrmn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xfjpzjlr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgdexxid.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pdnawxct.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3voawdhhq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ansfyzwv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hghndqjj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3udghrghc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lcblciho.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjxndcpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgniwloy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbwrzsyc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mgfmhtkp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3qmsoznzs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3saqrprnb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bfqhgdqr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3twlutagz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tfblsxpy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ckylibhb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3edmdzabk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hyzcfcvg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmbacyx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xaglthsz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtzeuwda.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wrjexghj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mwovnrot.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wlhiymgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfncccqb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wvgxomkh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jaetkwmq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cwhjizqa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3phuvpkrh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hpqwandl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fwqgqjml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftyibvuz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ymrxectz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrwiwpya.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pgzhwmqj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nfftcjtr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3afotuedz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jsxdnsqa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qsdqrqpf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3yeeecczt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3uhpzyhqt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3muexmema.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dgfqorld.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cpdcmxrm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3acrhjndt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hungxtwk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cyhllqib.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3daslvxwy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zkuzqabt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3sillmeoy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3maeoljvg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3oweiqxzj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kvrsbgej.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jpdhtlwu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mhcgfijn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nesfkswu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fmfoiait.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zrinysho.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pamcgcwn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3irgrowor.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3roedbnme.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wegapeeg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3skalwycu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3psjsubyp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xbnawpje.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sgfywnlh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bejtrhnj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhsqqvx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fgucvbbo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3soyvbvdr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mwtfdtyo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3goodmbtz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qjbedpkq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tcrggcci.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cwvgjjnh.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hkkjogkv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bipsvqft.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3zhzkhinz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zgojezdf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ppniilhj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3eeumnjsd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3boqyiejz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uxevscib.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ruyicync.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vebpyntg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3opquhsct.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ifjaysrd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3styhvwed.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iavdlexk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3lfruofmy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tqwpslfj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ujdlvsof.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zkzknjwu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3sjnppdrt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bvwgpovw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3teaozzwr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fctxshib.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3tyiywtnn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ybexjzzo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3pacsqrlt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3huqcephd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hsydctgi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nhrygsjp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qoduiolx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3olmpqrwx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3akknwhyc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3aflyglbh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fidklwof.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3rmslwzcn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3homcugwi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3oyafnnrk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vfkikrma.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fhjdnxsc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gpytvqng.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rvnzwboz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mkkhjana.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ndstggvk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lnfcscmw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rajuibni.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ffilzute.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjuumder.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lbtwinbs.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gauujzeb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvabffgr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmyvfykj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ugsrwrac.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wcxlcjdj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zhgtmwyy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mywdnilz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjurqdnt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dwogkkzg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ydlyjnbq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yelermpf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzubimho.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dndzdkjw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cxdggihg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gipempbj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kcvbhzbc.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ykobkaev.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3txtexytc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ngbttodh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3enjiurhq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3nfdsilpb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fdjfpddi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3trsdntoh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uigwbvrh.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mlfeivls.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ghjtwdyt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vuwbppru.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hhdmgkcj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hgduneze.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xrtsijsf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wddhhjkr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zotmkgzl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3isbuuzkw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fbpemqob.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gonapbfc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3dkjzefnn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3qqamiadq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uowavtnx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3unkedrsv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3chtcovnh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3wpegkeib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wjcefwny.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vkbdltve.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3jsnemlks.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vzidoxpz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3figildoj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fkfsrmyw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3frdpdstc.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xppcgaay.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyjbebxg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wmftqnuv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3meclulmd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nexchlhu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3fequhnmm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ghhcjhth.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tjeuopmp.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qsejrtue.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nflramfq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bcvkdofo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jhwhumvl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hlygtltj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3nbxgdtub.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3trgwwkeg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3lcrkpihn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3idtzdpki.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ydbennsm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bofeziek.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3leddrlpy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ffrneeaj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gdwwwrmj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ootzwejr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wygvycfc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3upboyizp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3budctpjk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3nbuxmqrr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xppqgare.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hmpsioew.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bjnsufiv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3flrriopo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3wqcxbhwo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3hyvmmnau.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gomheaqu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3iuqtpalr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ydrtrmba.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nyaoytzl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3kilqfbhl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pohbcque.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mbuvnvpi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lqhaeubf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dskmlggw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tqwnhliu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pttxfnvm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mnurjkvm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qgrszcwm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ahmemtyw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3yxupbfew.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxyijxis.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nmspvuks.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wrnjzpvg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ommddwvd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ekemrxbe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcqymb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3iuervopk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sscuxovj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hwcfoesm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vsywjhct.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lhbsllft.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jlhgimyq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wujgvdcr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vnuannxl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3skcgeivm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3llrfmads.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ghycvxrd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3tkckizoc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hdhigkdu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3mvohfpne.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pnwsifda.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qsujoiag.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3cevdhveh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mbclekes.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ozyzhpbm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dmnyfnub.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ugbsheau.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3bgegvzrv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hmjahvoz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vrpxfefd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3odsmtuuz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ixmxawwf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ltoowjxe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dudvvdgz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3scnrhwbj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fcukmsxn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jhphdbnr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vrjbwtgq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3lytdesvv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3utghmkbv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3tdztlzeq.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gholpzso.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sevjdjxr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3seefqnaz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3csyopbfv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3agpngnhj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3iepwfwya.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yburuywv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3tfyadded.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pzxcfvnt.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3knugkanz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jwkecguk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3avcyokwr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wxtwdhod.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ujqisdky.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3klhlbhdb.html


<!-- 参考信息 -->