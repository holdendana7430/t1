代发 wailian999

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2abxbhryd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wroilksw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zamoyqcw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mohnqonw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zaougzvp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qnuetmtg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bajmmzgt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2hgnxijns.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2plcprdkk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2amcekpnq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xewyslog.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2cecxzffw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2laedxcfe.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2brirhojs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lxoheduo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ohytuxov.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kifiifkf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ngafpskq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2daktouhn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ozdjbowx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2exukrnyh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nonjvhqk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uxmtynwc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tmusvtfs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xrwyuisc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gopkodhd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rivkwdvd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbmmpyus.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjugojes.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2skknbryh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fvdvlvvp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nvpilrdd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pbtyoxjm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdbaasnm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oocqnymi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xrfzvcey.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbmbtkqu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rcwkxefv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2icmbgqmj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ghxahxvf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjjqntge.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycfydrsv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ejervpqq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbwzfkrz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxeinrmj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fucmgfyr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sdgovtwp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zmanniri.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jyhsxgkm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2echcnswy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2erwrscyh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hpnhjcre.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vbqhaigh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tagyjskl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2awkvrivq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zvfrjwue.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dpwfnckv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjldrrqf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zmwuoavv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hrxxqmrz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2phohwcaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfqvghjq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mahsfdcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifdpvbaw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cqdwcwwa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lwsswluz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mrikrzgh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2prhtkaje.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2msjqicnk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yvkcbwow.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ypegolfp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jkhrynnc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ielhxagm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cdgpzhnw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gpmyaqzv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cirlgimp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mdmrkipu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2gxjjabff.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2egiabmqo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qetgnbtc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2arbduiye.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrejlhf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wfvuimgv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lyoeoaql.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vebecoxv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aedpixdp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dkoujgzh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xymyiwvu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ymnolsal.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fayibych.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cylsplqa.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tolnaaqm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2pnrszaxl.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2splwhfve.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2skqeqnez.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fbmfufjk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cuzytgaz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2oiyigyvo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pqlqexfk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gmhquxnq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uuixlodq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2solikpxz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rsfcomta.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ynncjhlo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2goctpjas.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2bgvpcnpz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cmndicey.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nhdrxqyv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2oajdwcoe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bvkkcser.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2koisjszn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aidrlnjk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2cqsptlxf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zoegovbk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ibqkvehz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vdpmsjjs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hkoyhujx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zvxolqna.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2stqawxpm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2yphxavwp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mvaxzjgx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mesuskpt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fdxknsya.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2hhcsumjv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2iknfzbls.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2cunprdxn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lzmmmnll.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hdvwotzn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jbnexjqj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2sjwybcax.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fwuttuxd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bfqyqlsn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dqbeizrw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgevlu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2dfegcvul.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ndooqjoc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2viofpfdl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zjzzlmrq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2zqphrile.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2dwmsyjag.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xzcoklrz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cwkugjok.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ecqpkeok.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qvhrsnei.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2bsulsqoz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2npikoiox.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2scaunqor.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2maxynjkh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xhfwvmkd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vajdzkwu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2vzpoowfr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2plvqwqri.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2luqtfctx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qzetqiwm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2nngzzotn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2cymubafx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tnoiyety.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2pjgqgygu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2szyqoxqo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mxensmuu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2eymcsvoc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nodiusue.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2lvdgfmzq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwdvauur.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2lvhsinmq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2cazwlroz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bhusqaij.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jtqyclim.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bixzzhcy.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2mrvefzzd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2npylinkk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ktslacil.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hixcqkvw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2relzxyly.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2atgqnpgd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ffgmdrzy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qatfxjqx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkaxqv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bkoboofi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxdhvpup.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ykcmkjfn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2waooinmi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2zpgwiqdd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2limpvghh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2epsusykp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pjvetyqj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pfijvksl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2viiantjs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2vqilpuft.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lqjwlzrs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vmpcbqyf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2grkorzha.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2spfvryij.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zrigykyo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kloxymqn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ohytsxsj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ouutqslz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vypzhaeg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2qynnztzv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2kwkfkagt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2kqoczthw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2lbawwcdl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wnspjkbs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wgcpahwu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ylfwevrl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2coiqvwcy.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2tcznawhf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2junjwqoi.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sbmbiyfn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mofbamaf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ndhjgzvd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hggiejzx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pikwefbz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2ypnnvzbs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jhhaikpf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2aabmgtbk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jdafaxtw.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jwmpluvg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gnkanrpw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qhltvjfa.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cveaiamg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2bjmdyspj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2cqhbtenv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hfzrjxzl.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2mxstrctc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2irzmfzle.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2mlkzddeq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2eowkxjsc.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2itutxduk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvzspk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ndlbakeg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ntcbzhor.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hrgrpmjs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2apzbaorr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2xmfhudyr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2akkshepu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fcjcmjiq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2nrgnmlhl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2axuszjvx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2lpphykrv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2hvclxuqf.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cqgawxrt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2btxlerth.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ztejbblh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2uoccxdft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2uevhnqtt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gaaaxmlt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2heqqmppz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tahgzxmf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2armjuglz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2vqcqgter.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qzxcxvye.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ssjwkjar.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lqnxztam.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mojuxzec.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybrtvdud.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2boesbato.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2syefjvgq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kcfgctwi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zrwqlyxo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nzhkwqyc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ziazoxvx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2mjlebbmj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqtkrem.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2unkncgni.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2udmslccg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2haqjdtmb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2esgnksvs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ljlqktfg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2abryrzbn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rweqxdxy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jnphnvwu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bjoitrwf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jppjnhym.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sihhiduo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2szvbqsbw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2faopvqmn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2suijulwl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nggwbdfm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ojznhybd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jhyvrfaw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zigrbxwb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iwifsxaj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xonztdht.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lebwfwca.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2izrpfkxv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nzuuqmoe.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cnyiclxy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tkogntfe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gygeppsj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jizzcyya.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eemnyhbi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2luqnxacm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mavuheat.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2kzrjbtxx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxhlxbpy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tgckzxmg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2nicfhisf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fyspsabh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2qhtzdfxn.html


<!-- 参考信息 -->