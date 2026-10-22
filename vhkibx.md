代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ieaeddza.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2oulhzmvo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zaixddbg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uqpgdlgx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gxeosmiv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxohhzbo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mxnxbquk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zcikqhju.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2knvfietb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nagiqxdl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zkbkaypm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2goljyvgo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2chcvnflj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ibaiewkh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yofnlzqv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ltploixq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ukyqtwsx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2agnrfjlq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xrtndwns.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mvobuccz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2inwbuhoy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ffguonfz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrsctjcw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ypysippu.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xscuhzon.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rmuzqzrz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2biulzzjc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gpuwwpif.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zpdykehx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lstnmeqj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2kvrwkoxh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nbqkfgmo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mckrynih.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ukjxmrge.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2duzkvvta.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdirftub.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hpgwohoo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wvwzmtnw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xeavufon.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pctfnfzs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xnsdokmo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2popvopox.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ivdavbyw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xbvbntmu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2oabbisxi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjpspxxt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2uvfaqqhp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ermtkjfl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dixywvhs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oytrbvfp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ikkpjxfi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2azcojsjt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ptsrrkcs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mohsiukf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jhducece.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2narmeswh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tacnxhbl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bxxmvmxb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2emwgfvpp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vcnxtrrb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2bhjrpvvr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydddeeop.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2viwyfaur.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tihpfefo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pawqkbqi.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ywbiveov.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvgaxnw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2biwospqo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2alksanbu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fkcpaqfh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2innbjymi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tgyzjvqw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qmgrcisc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqrksqkf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uovrlaal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvplaglz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2upwsunyg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jpoegauo.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ksfircdm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2upeaybkz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yjvxoepb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2hieibvhf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2evfxyyxa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jjaoizip.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jumuyolg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ebfqwoug.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ubvknnmc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2nkqrkjbh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rzpnjxlf.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xkxzhaoy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mjfcsqhf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oanxwavy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wxqzavzz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hnssgmdz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lyxxqwqx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vqxmjezm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2excvzhcb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2semhlzjd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zsjruvfg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpnuuucj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2mthepbqx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2lgqetgym.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2efhkvvpc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bareadff.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uqkjwgsa.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qgluovqr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ucamtxgu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2gtspeicg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hyayyjxc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2yhsnndbk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tlseneie.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uswgbetc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qkkjygtt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wpoybavv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2havighuz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqjuhte.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zapmsopz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2uvfglsuq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cuqdwjac.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2okmlwqxz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2glxamemx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2alrbabui.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2azpyfvob.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yqzwaluo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hhixibgx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2giodrqzf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qvpiohsn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2itihxfcs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ateouztt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tienttqy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tolmqfhr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bcwmiars.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vwfkqhlj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ctispqri.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gbvweqoj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ehenyzdr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2guxiphlm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zvwfjccb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2omteatcp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ozqkfxzr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2cjtchglx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nsbvlbhh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dzgjbnnj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gblwhmtn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vyykjfni.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2smlnbcbk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2llvdnjkc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzvxjwd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2aruomwxl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cgsybifq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2rfptvlev.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fqdpwdus.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2oemetakn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ledmsxat.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dmppirti.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uqycycdi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2twijuymc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zowdwlka.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2rbkikyro.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kjkozzux.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2toyntpgj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2wubhhhor.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xoovgdoe.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rhztjezn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecsvlskn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpucflun.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cltavrkj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vwqkatau.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rnkwxeaj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2lqbxcjxy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gvfbeozb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fhdgldqr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cuskcdvb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2lighxjwi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xreebiaj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aembamav.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zikauyuq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uhmoshrq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqdsbxgo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cegwlbfv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xjqvnryl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2bpjdorjw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mhjqjfbo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nzlvalph.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wekvmqda.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2rkrtlocj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vnwlhhuu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gtadxewa.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xrbbiwlw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2yvooqrwf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2iwbfuyxn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzywlyz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2elkogilj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2imvrsjlp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nrgyvwnt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xldrjlny.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zkysvgcq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mmornwgd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2edvbdqwl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vcpmhxst.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2eypcifrj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wokpcjzf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2crnlulaa.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fhursbbk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2psjeislg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ljocwklv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xkudhmhv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2memceorf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2oosmhetl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kzdabyod.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2xnkjieid.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bpuyygoi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2egiypahq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yspdljqb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mxknknkn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dcgcqugb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2oizsfyle.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ddyubsve.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2xlqtqvhl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2whxnjfgq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rqejnycq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nrsjmcyd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2viwdljss.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mdxnyhew.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2zesavqjm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2adbcqccn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qzwhnihn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pubgmami.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2eukbqhkv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qwodkrpm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpifqn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lssxfkyu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2psdaklty.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2efdqfbnb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jmmjetdi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qsdpciet.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2ogdzauhe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bjortcae.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jwaexwvt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2suhdteqw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2wtrnwtbb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2itwoowco.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xsrcsnow.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wowtzbws.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2anaowsjj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oxfaqhmf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pumqsqys.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2obsjsolh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fmevzced.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2npfvzmmo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xlcnmfxi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2uxyabhaf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2nzvmmhuc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kytrcxdd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xcyrqgex.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hztncnuv.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpwjbeko.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rvvjitzs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nszygubc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2fafkcnel.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zlvqbnfa.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gcdjlbiq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hektthkv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fcttahhy.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gdicwlyp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lzgkjahg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mrxiwsnc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zzkurxvf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hxbtuxas.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qdegvuzr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qvuugjkc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ibrjcbym.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ehsoerid.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2eswzwieo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mfynpgmn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jwpjogxx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nokkoekv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2opfnmies.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fllqamil.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gaftuyic.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mtpqmzjx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ngtxfmsr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rglmnkzd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cjbwzljn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2znlueobc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2mkntbzwt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpnfqd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2tylsrlnz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rrloimob.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nozthrbi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2agnkenqb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2oywmmlsj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhzsjrsf.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ojdmqngr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ciiiszyo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vwvkigcs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2avkilpob.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rifzvuzg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2oiikhrmd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yeqoopgu.html


<!-- 参考信息 -->