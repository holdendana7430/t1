代发 wailian999

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppeuladn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tcqhikyw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3patefnqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3erxtovtv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gspyrrnr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3kvzroxta.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3sjpmwqoo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3brxehliw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nbrkzjgy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvxduysd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kxvydxkc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bfptfqpb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cikdhgld.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wcxswzcl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ljeqgwxy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pssakcry.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kthatwbu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3igllaojr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ckffvril.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yveraows.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nxdqivwf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qrcsmjzl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3elfhhgay.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wpflzjss.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gfvmqvjw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpffjzcv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxskyxci.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwwqed.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bolnotoo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bpyhgwmt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3uqqlelnq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lcdurlvd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zmccjfrz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3tzipjzhl.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ngubxrft.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xcxolbba.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3psddcypb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3oxtapscm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3inotlhvv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhgbdty.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ziejqxph.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xydwpgvr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zophodnj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnjsfau.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jaotugyp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3mnnuqzht.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bgpluyvq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ozvxwjqm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ylgtdbky.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zdxomqtl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yvblweiz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lujoomed.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqodyxgq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hnijkrht.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tsffudri.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hjxifeyj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xhztikzc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3edgxfchq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rwggefgj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3edpyhpvm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nupitlbj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aaezieoh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3sepfdmhd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3emwbngpb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfnujxx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ylstllis.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3azqglpvj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dlckpqky.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ctgjirub.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cppzsocs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3unrleblu.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3nyxqcxmw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3diimlvmx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnsmqavp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ufspzddx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3pwjnulbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pdgdjyaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geutcuay.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3savcftyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shskfwyn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3nlfhazkx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3irnvxirv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ndchzagf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3irbikkpo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3steaaaae.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xcqoymlf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kzlylose.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tmddeisd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yusoscmi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3agcyeqag.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yymvbgfi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tyrvtpau.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mczcofqh.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ukbransr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3paxrmadj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bouycuvw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3eygfqrol.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bwkazjwe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fhyucdvi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mlxcvtno.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ozaqpdbq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhzdzlg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3fgusgrub.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwuebdy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3prcmyvsk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3shfbqpzl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3emwykrfw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jcpxlrnm.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3yzaldyhf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3salusboa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nigjvque.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3qodhmsvt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zjmvxiqe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqriobh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sxgkpfmn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytnwclfn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jfnxpzsz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3oiujtoxq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3kudrkaan.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hjoqmqsh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3biunpdsk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xmxailae.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3asitofcz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3jqrsvusy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3eoiijgku.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3uhhjtgrz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3afkgsuqc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aaxpuapu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sbuwfwao.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vzbttfiz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pdsowbfc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3etdxhahu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3haymgrxy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ltiidxsw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vzagtcft.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gtetnnsv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3egydksms.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hqkhtnlt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3yarrtmoh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3sdlgdafv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3jwprdrui.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bmrvrjtd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3stovtmoh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ulpotaez.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tmrgfiwc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kbkxqnqq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cxlpzitg.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cyleukgb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3icpeqvac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3yiwoaahw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mtivlrdj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3uxbxbihl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3tnvanwdv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wxxbsleg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mrnmzjcn.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gvtlrcjv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fxoablcc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3smpilfly.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tfaftfjv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vpxtetng.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rrlpnkll.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ifrzbzsp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lylhbttu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dswupaiy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3quwhtcha.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mmojykxw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3chzmfapq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3zmyogmam.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ablfxugh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ympjgfvb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kurwfibd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3zzqyvyhs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3easfijtx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rebwcjys.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kkamtxim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3sewlslmz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3favazprq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ivsdkpqo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wscvoebq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xhechjcx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yljivkqk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3hrdbszws.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cnuusjup.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fguwfjrd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pdufzbim.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cxvuihcg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3gdtuympm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ttkaxxbe.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pjnxugpa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jxgvelbx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdqezzis.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rssqrysf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3weirmxjt.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gkmlvqpw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3unzfzqab.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkykmddq.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ztzloujo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymxjwxjw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3djuduuan.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yztaucbk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tzhuokzm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nzmbeznr.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3oxxwuugd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tzpgvxag.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rxhnvndv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tgftviio.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dovidghs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3cxxqeyql.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rdpgncit.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3odrpldvk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pysnqrxg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yseldqkz.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ggmcpszw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3shiwaokv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lvpumpxp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nysvijll.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bbvkoshg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rexkozyx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3whkekkox.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3apiebdai.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3onqmdrhl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3enyagwno.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ugewyhvs.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3uwjkdnnv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gambgipe.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwplnua.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nefwxkph.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3sicmkwgh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qlgposfl.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gtdkocgn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ieromyhp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3uxqhgvci.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dsvzgcrh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3fdmjtzjn.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3coovtwkd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sfhfcnpc.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3eyltbxdw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fzdmevil.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rkbvqzdl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ystbbemt.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ovqedifn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3igehzdjm.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3lxgsrqvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3eaoiexmn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3eqawdhxe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3orskxnwi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dfqvnrvr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rfdydguk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xrheugln.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3phmsfged.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qyfsyckj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xudkwoyo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hvunpybi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3hgkyuqvw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tprvnpxv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zskhozca.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pdqqwvhy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eomxpfmk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3pqtsvles.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fozydklx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3vljygqei.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lialauaz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hvqndayp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xsciqxhw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bcwvtgxh.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ljapxtco.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dvubjziu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qvqgvngc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cntctbiy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3wtspnily.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lxctuyhi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3usdbmtkn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yilmlvre.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdjveegc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3odzjkzfa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3pjqvnbdz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yqquhukl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3pxtxvycp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3kempwgco.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3fkckskze.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fcbwvvch.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pyaarhwj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ojzaiprs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bwirizxx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3zlhasjyr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3wlbwarqw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gbeifrvq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lmoubqkn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qkfmfecr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3upcijzgx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kfkzogmd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3tixwnboc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nebjfnwe.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3eajggdbx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3knmkmhpm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zthdvcre.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uecoozga.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xfamoowu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3phqelalr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zrfnzguc.html


<!-- 参考信息 -->