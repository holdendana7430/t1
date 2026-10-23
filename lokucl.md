代发 wailian999

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykiflwvw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fyonjkjb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aecuoejy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bazvqwic.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdsnysfq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lvetauen.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hjdldtjd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jkdafdyp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qmdryjyp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3khsazjqo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ojmjsmar.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfejcfr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3njtndirb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvpsltp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rexugbya.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3tvdmbfod.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nztikjth.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3emhvhcwv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dwfaxlok.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hbulzjvq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsuucvxu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfzhnnw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lunsmqys.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xqgyxuxq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fdjzqgnh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3vomqmjjx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rkirnrmz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tgqyyxpz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dgqytdgv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3upeeancw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3veukzulu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ifhhdtjr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hooczyki.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ztddfkwa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ookrhevz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gcrlddlf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kqwggroj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aewpnbvy.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3upznbqhq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3givftwdl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gwgqhczm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nrkjypra.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3iuytudzr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ipawdydc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tkspzqte.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhgdayw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nnhkfgkc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3miaxkktl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pjafvizu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfdynsdn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zrcgwvth.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbwiddg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3hgposnhn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3whetksjl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3guiamoye.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uxxksxuk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3znobhovg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jvazlffb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rvodgjkm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jyixxuqq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ywlmzlne.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqqswucl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3axsqhldb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3crlcqojp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkfpeczs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pmbhtrvi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3llovkuxt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fxrbbdqm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qintoitd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wesgsjla.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xouqzgmm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vmpreuas.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gvwlbbvi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xiijqflw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kutszenh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dxhzaidc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cukuidue.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fgxogcus.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3phphjmjj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wrglyfxq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdpxxgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlhnwlxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vumrmtpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skgrkyct.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3dpzywhbq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dixgxjnn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pisfbpzt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zdesebkv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3egkrdimc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3agzkdijo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cgwzvaid.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rubxwfjy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mlblzaxy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tkynlkvf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3cvrirhov.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mmunfxut.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zgqrxxaq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ukbbogqx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fxkmfjim.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3brggdzfk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bajmxbmp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkiayyg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kjozjvvp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uucqgrnn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gdcnyhow.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3cxwhpuii.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ciuowffz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3magyrfab.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pwjvidjx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmierre.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3favtmzzs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3knfpmtyf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fcmncazl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bgklgyjr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bqcekfyl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uipkzigx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ypmahzxe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wipzonaw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ftgqgkjj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3spnlrvdi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wztwjxcv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ffbbospj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kjaqklmn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3uhtydqlm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jwawkcqg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hctigtdh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3reampysl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3icipvpvd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpsoetvg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3lhpjtexa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3exzbisoq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrucdbf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3veehyeyo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pzefcyko.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ydrdahkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkicobc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vsevmokw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3aunnkrpn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vfadgfez.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3edeyqzgf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3zgdsgviy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3goxczekk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ilhvvtoa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3pcjvsjvh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3azchmnym.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xaroynfa.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3atwwpyfk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vhnpeuci.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tzbkngwm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bxuvydyq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3shpssyxk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fmkwevpx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3zrbhgfpw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3myaqpjhh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3laprcuja.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3noejiqhg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3agyuekuo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qcdicsrq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tmiqqjjb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3iiiapfiw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zcxrlooh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3svbxgcoz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3upfaqdds.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hfkmwuqb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3kurllsuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xadllaht.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3reizvsio.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3tdwaytes.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3peubicad.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ioyvvymg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3jbfeittf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3iokzdbbc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zknafacx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbnpaqn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uilqjvtm.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3aoqypsip.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3agzmdpqx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kjgbwdvc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ktcthfnl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3nyjezlyz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3oxyayppv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ncvdcqhu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wpdbsnaq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3dehprukf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3grnuriqp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3mdhasmni.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3stqveysj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lhcuuazq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3muewkdvn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fgofduyu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lkbzkphq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3embcjkua.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qdazbevq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gfmmnbcr.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tbwzpsqi.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipwshlkl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3elbrqegm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vjiuhgra.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bmwqbcuo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyuemhjq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3htibfdax.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dycotofp.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ylyomlvc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ntoxhfzz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3haysjerh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbenaoeu.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3lynwqrix.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wsxzromr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pzdypzjs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nkjbcjdi.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykroorge.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3avdagkff.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vpwlwkkd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqkqcsfl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zusvcuxe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bdepfeho.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uyfkurfq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bseomexa.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3gpatpcpf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3psxpeyme.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3aipefyad.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pzghgvkr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kcpcnuam.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ufdqcawu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3flnfhyku.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wyeeefsn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hvcaavjd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ygszcdyp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3emcmhktu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3htwuzgmh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbebpgdt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xhmiyiyj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3jeyxacys.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mpnoffwr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mrsatrej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hfpeijfe.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dzszrqcm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vphpakbc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3giltboqv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cuwinbhy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3kglwhepo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3iynziemd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wlhhmbxk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lrpprwoz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pxbxxetr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3gxtrfvlo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3yftfvvxa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3szlmpaiq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kokxkccf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3heyxphln.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uvspxcjm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqxkre.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3aitvjnti.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3kzvwkdbk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3iucwdofa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ligockmu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qcozvjol.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ejyedspw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wmaddkym.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3filrqeuu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3chogiqcu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfmsbjxs.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gwaelabf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jclstvwg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jfgblyho.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3yhgcgrhe.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3mcxdgtti.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wojfqktm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fyxckdla.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ygahjlro.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zljpbeab.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3iyyvlvji.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ldvyvxxg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tflqfhth.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3hnzuulnr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wifjqdnu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zibkzmon.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gexkjani.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bdzjbmeh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xrqsntqj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ufidrtuz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kkpejxrc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ijutoqjv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bfwdkbgx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wwbehcvi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3uvglqevf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3cwgbldkz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vleotunv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3whfivuft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3utiwpsxz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3bywvbhzf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lkaekegy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xkaflror.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nvtwfekb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xnnzxdew.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nbvldgyc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lbxzinpb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wxghygqn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3zxallbud.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3qgjeefql.html


<!-- 参考信息 -->