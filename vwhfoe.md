代发 wailian999

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kpoidmwy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vvadohfu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2umknomnl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2paslwrut.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcydbrzh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qsqkoaqa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ynqctjym.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kknylicm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2petcojfv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2gagxirvl.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lstslgbu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kqtptkhv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2loqobvll.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vepzytmk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tnrqnvss.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2quwlcquw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2laudptbu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wmwduodo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vspnjgbg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ffprecmn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lsouvfup.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqbagnzn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wglbyysn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2txwvluri.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2uutinbdd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kqbgewvt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rizqstyc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hzysqhwk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2igzjjtwq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hshfrfif.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qsgdljsx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ewcuuddh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2etmpryez.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lhpcvxcw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ggmjjyci.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2veoogfhi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2boikctqn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yafqiiom.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fazalcde.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctaammll.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2zzudgsux.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2icazvsts.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xaftmesk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dlwyrozm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wkbjrujr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxvvkn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hqtxjkjw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lunuftrr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbryhrlv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvkmlfpz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jimycsbm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ifhwgjuh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jtzjoxlt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mcfznhwn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2heummtmu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2svrqhyur.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktbjlkqt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jeadddsg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2swodxdmz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fdvemyli.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2tkuxeeaw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iowgidet.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rpylragw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xdoaszkd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zfwmhdxa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ldznfvfg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lxkeumrs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zishqlnt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nonmgoes.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nbltafpk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2awlyejbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tywknvyo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2uhgtadqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skdccmby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lzwfeuyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwgmhxdu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2uhnoiqaj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zdsmlqwv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2hjvxaehp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uoyzxqwu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yqlfxtrk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pftoasui.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gnueqgdr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hsysxvuv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tfrbgzkn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wvujlqbq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ttergonr.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ogceaeub.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pxbfacqo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2qbgbpgeg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ofsxfwyo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2pjjzechz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hymimgnu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2dqrvluzv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xwltnzon.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cagjsxch.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nefdadxr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gvcvtylf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ulmihtcb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiuivrsc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wmrzhdkc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2mkxwiiup.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2sdateyfp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tizjhqkv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hnolzzrz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tmuobeju.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2byuhrjss.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2tkorzpsy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cgqixfiu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vvsmedvr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pwxbfgbd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lbtnfqxl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2xvrmynsa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2jitqtrhx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wtgztobs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2nfevyvcx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2elqvxpxz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ghqlbgxt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qacwcavv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2cwkdowja.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tzxldusi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2nwqfflbm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2srtrwgqt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dklgymzj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ytmfsjle.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrdtgmc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2noeosnez.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lwtrlshu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gfjdocvu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ioxukcps.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pjzxgbil.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2blofazuo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2aoyadvft.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uolpmkef.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pgcxekrk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2drircfqj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2juzbvczv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2fsxfndvi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iyydspdg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2hdiircfe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ocgzsdbk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2pplekebq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2bavgixjk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qjlwrakv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jlzrfdpe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2usgoioge.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pplnobgm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zfqmaedd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ngosjocp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ydbmhvfj.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ocrmurfx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ysvubdjk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2glbjtcxo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qesrxelt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2trbzuxdv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2quxzdcfh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2emrkbpjn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2djoqwjxk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gcooyngy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qtgftowk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2opwlmzfj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jbxhjtyo.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2bvvrhfsz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fntyafwe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lyepuqzx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2avtisbqr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ycvofvbk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mevostmu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rczhocum.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ztgvuhma.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ingmaiyl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2hvpbvnta.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2amdnaprs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2eywwxfuj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2slsymcxh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehuhgfmh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ebrkteqc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2asoiiuyh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2btnettzj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tuyoblgz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2blsmtkdi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qcexoqbo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2kdycebyv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2avvkhspb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ivrkbqem.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rsukawll.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nbjfrngq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ndekqmlq.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jfjlajra.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2cdpiixgy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ujgpcumo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vkhbxafp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhwxzuxa.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lpovebmk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ofoekldp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2beruqqfy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yrctajyn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sennoqas.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2rcjtwsvx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vqlulbia.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2qfdxbbfw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2nziortsn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hfvmfaja.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kzoegfho.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ijivdalq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tqfpjyva.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ifprxlxb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wqimbrde.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cbsivkhm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ajazjeva.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jabozflg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fvpfohgi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2zzcsqbvp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2orquoadz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fpyjrcaz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2fvbwbiyp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nmnjtsdq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cxnpglzw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mzcfpkpb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2aepjbzbz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2icrvehyw.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2loupxfuy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mbsoxred.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ljdphhyi.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lfrmdala.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zfybmvqq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bmrhcxcj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eknjfelt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xnullylu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hqcmjzud.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hfqoloxw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ckuqzrot.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2pqagafub.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2upsitmps.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xejeaxzw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2couuysxe.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2bendrjhr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ubradedi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2escgwiit.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ezzcxsde.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2osbvlxga.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fgdmixqq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xrxxlaka.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2zmtqzdvj.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2takqxhfy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2trtjwsoy.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2trlrcsdk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gxstcmmr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dhhchduo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2vtrbzrhu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2bodgudcm.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ajbxeghj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2zumtfnfy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eywekqja.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2totcjxcx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bohmgyec.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2naubiuyy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kvixsuvt.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xpmomkuo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yqnccyiw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dsstodjz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2declqvgr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrqqnhue.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hulasfrg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2selzqtph.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qkizocxw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2bphzpktb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eslfgkbb.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qqcqmlfb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pdrtrusq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wmxcssfx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2usolvgnm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2euzfwxtu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fmoliqjy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2zitagxpp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2optqnzce.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2gmmyemky.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2owqvavku.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vpiiuwig.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2prlhdrsn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2qhcocutt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bcvatyrh.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ophwehce.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hbcrdjhi.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2uiqupytf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yprhlnfi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fglbhazl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2osfwfnzo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qcedeepx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wsoseuhr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lhdazrsi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fexbqyrk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ycfzjjfr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlmxrit.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2mxbdyncj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2igdopgpy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2awfqgorq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2rgqjknzz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2veuptmbo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sinikwpo.html


<!-- 参考信息 -->