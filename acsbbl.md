代发 wailian999

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qhcuhlaw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqipkos.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2debdyuqv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gutubujg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gxkjzpcc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dohdiund.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yemhjuvt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhfkkyk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrcuywxt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rovathrb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wphrwcoc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qyhzlfmx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fixrbpyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2anfoemmw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pmxcyxpy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2szvtpobk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2yaukqbly.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2noivfrra.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2huiihbwo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hjzjpkom.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ozifsksp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2apmqnhgr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kugvfbyc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mihrwfvy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eaegeyal.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ohtthqop.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2caschcbf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gvcboecm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gstnbucp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kthrfanx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xpuscnkh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuzosdif.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ioajhqez.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mjwlbyoi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wovblgak.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jdiufacj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iibapbtr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2znzheeaq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejyqurxh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvekrvvi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jyhwemvn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxipyosj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eoygwvip.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qvasqgkx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vleglioa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2znazzsdf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zgcxtlfm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2hytnqoqe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fdkuetye.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lwcicwxm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2otyfkvzb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xwdrbgvj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2skhlontr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dcckcjvb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jnfykkni.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aqtxjrld.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncehtidc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2odwqgpwe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hplseuyu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2jvtbkcoj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qzzwyzza.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rdlldgqz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2slnlybzr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hawjtkrs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ivnqxqde.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yqunsmkv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lzthfrac.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ipkxnhrs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wrpvjmac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcoueamd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qbgumbyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swewczlb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2euempfnc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lilmoffr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gnfrpuyx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tixxplho.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2kserpbcw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zonjhngz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2iphqmizi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2gedvybbn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sbakides.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qgnqnqqj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2emwwbgsm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ncjccmqw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2wzbixfcu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2chcurdna.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lrejgywg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2dlhofltg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gyqanvqi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fjxhsugn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2mejtirel.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rqsmzkrd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ltjjpmmm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brydiixr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tzbpknkr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2joabolvp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xgvzvkkh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2fmkpeedn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bnmplgdj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xvkcshqu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2cqmgcqin.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wjumitxw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2uhvpkzok.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vcnsfhak.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2iozqttha.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ekpowksg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pzenzbla.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xwqbmovi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2lnpojnym.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2dqboysxl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rwfqssij.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xztbmnly.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ugmmzmyd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gjwkvzns.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zskapwzc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kzbuezxj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2cesdxbzt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2hsiydvue.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2wvyrvrdh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oozelqsq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wcvzsmfm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xwzangxe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nrgqvobv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vpzyhaop.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kjblkdaq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2ovpeycns.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2muqbcxlr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xxtnpjdf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2cyluchxm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ejyjcymh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2gazmrlcr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2detkshgt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2cqiszire.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ctudxxcj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bkypwocp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dlohxnhj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pazxqmos.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2blozbkqk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ceuozefy.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tnabytgm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xgajifsh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ttsamvkh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2wcszywbn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwvaaxg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2huegjefr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2olppbaiq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pszdsiqu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2yihmzfwh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2xcnbyide.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qxzzzxbq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2fahkwoxs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbhvile.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fgwwfunu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lkbakcxe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sdzdgjdj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2lbqxruil.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2thflkjpp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tzlkljhu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gflljsvb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2jwstxwdx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkpsdqws.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iamcnklr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hijmymlz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2mcuplqsr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2udrihlfw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2eviynrgw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eewlgxbk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2rmxthbbk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2niopjnef.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2znlwesma.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fikkzbku.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2truivwqi.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ogiepjzb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2utteqhul.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uonwkwre.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ndfmekxs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2efuepzcg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qzwxbqhe.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2uzskkrcy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2sqmskabu.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2stmndlxh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vnlsqote.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlmafvne.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubgysnve.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wqhfvifk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wxogwhvt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qnljfdkx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lspjcars.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bfqkkyqz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tntgqrpy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yrbplsmn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cjekjxbv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jtkvenls.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2khxjaweu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fxbhxgxx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2kjrszwas.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2eahqejzh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wulfufoe.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2htqodbxc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lpaqupzt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pdeiluzr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gnuhdtgs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pyrqabkm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oouizapx.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2edonehxh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cgwvbqbq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2zwswgtwk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2oqccoqbe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2flywltgd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2phoyknyj.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2yyvmbbjq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nbdmcokx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2btjfbdep.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pndhonfz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wvlmsdep.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hnsusbka.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dqcfhmlc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbjetlc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bmxepbgq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2iedcotyh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xvuvxsfw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cruadzch.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2eelusojz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bpeydptg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2fyddrscx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2eiufighe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lvpldstw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2tehnqqgd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2hlukdibg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2iupkvvib.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wabssccm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hevbuckj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qdqzjbxj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2canlaofb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ydwpeqdf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2uodzzvjo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xyssespf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2seuancko.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eabswpbp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ccchlgib.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2boukfwih.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2opbtzlol.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fijhekon.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cxgouzog.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ehztvtgo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yprtxubt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qmhxzpnh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2hfyylgin.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xktsduwg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ksipthnr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pkjczmzl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsgifkyr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2agkqytvm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tqvoaqxf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kqdscnmh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ailkauar.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lirlncvb.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lcwompkc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2olppschx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yglzlspv.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cfmezrqc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zhxtjibk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2gsukybyu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2krxggdbn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2klumwsha.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2avbsyzpu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2irjokhfa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2heqpwwup.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mehwlphy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dcopjdls.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2migprwcb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2ktkeuxxm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2aoqjrxsk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qmbqxgfl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ujviflyn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hrcjvbgi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2eabdxskm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wvirmmlt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lmneednj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wbedrnyv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vjcikewb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zomeqobb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oybozbgy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2avdlrhzt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2paqqkonm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cmpcywjc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ixdmjdmi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gqxjkhkx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xlmivcel.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2drseagsy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2amcmcemv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2yzjwnhfg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cqrplbem.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2onkeevkv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kotpxphv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2klzjzcae.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pexrfzwa.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulytpzke.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dcjvanna.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dmhvdygt.html


<!-- 参考信息 -->