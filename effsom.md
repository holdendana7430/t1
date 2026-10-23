代发 wailian999

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3coyfuogc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mmeqmwuv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wbgwrgpj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdafxma.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3osrmwysh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3omubmpqg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxkujmec.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mhyddamh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xhpkuevd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hffkxljy.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xljoblpw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lsjecgqk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aoqgszhd.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3smlfepoa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aiuhshaj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3toslncwr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iwwmdlkg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lldjchlp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hrldxedq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tvtvtwuc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3wjnyilli.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gbrgwjui.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zfyysbqo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ofkbtiba.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cvmvesws.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fsxhebnv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jnnkdoit.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhsgdwm.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hbmmzsna.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3viznjolo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kvyopngc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzwtsvp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uacmzpdo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xjuxoqqp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sidyxbgs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zcdcyuxj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3snzrahvm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fllitrqr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pxaavxhz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3scugabbh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oomibpbg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ljvljdlp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iprigdkf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvownsbi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wpqluxvi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ficwpgsi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3oqaxkuwh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qydwvujc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cpmxcvsd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfxcurzf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gizuusty.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3oxmxeijn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tromqxdy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wkkhedmn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3tuludfpe.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3apxnxmwc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gpnqaaiq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dddxtblc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3hihgfnvr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ugkctwgb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iznetpoe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jclklfin.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhegtyqq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fvxfztyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tqtikhre.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ljeefqtz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pxrwzxgz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqyxqhh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svglzpxy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsjzqsle.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jtwrovyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ulvizvhw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xkcbtgfk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tppefxaf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3awipmlnb.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ealymfey.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gyaxoyxn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fawpjrjw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqihlcqi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yazwkgsl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouwgnmyx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ymphfgzm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zjrfuqmj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yztdbzlb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3msajcoph.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wdinljpz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3abwnviou.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fqudxexx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zaavitwb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3aejezqdn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3asgzzwyz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3opuzgulg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jepamlry.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shyvwklp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lnleiuif.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xbhnnodp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mshlidon.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kxfytaxv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3csogmzlm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3iogziksz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hlikpzbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqezlytc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ktllhric.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggdomswh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yetkqxdn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rgoqwsmh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xcxnxyrg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3drwyfeic.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rwmccqvg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zdfrvqcj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bghvdevd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lxsxhzai.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3exwvqgno.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3petoojhq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qmtpqpjg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jkqapedn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3fowwoyow.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vnghuiov.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bxqnxgfq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3kvpcygpt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ozmzgdmg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3luvpvgmz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wgsjikny.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zainlxjs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3woqloasr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmllztv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ipxjctmb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixknjghg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xyrpnigz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rbrkrona.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jfgqykcp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fiknxzhe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3upnwffsb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3jghgdzqt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3frknddvr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3idgelafk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ycznfuyq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qdfvxenm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gupblwps.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxkpgbht.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3tfinxcwn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyoaguyr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rrhcpbpm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xvehjsmm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3eygahpjt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vyqufmns.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3apympwrc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vhmwdwcd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iabtjlrm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mxeikxhj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qalkjcfm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uofumoup.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qdrbfvpz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xnovjshi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3pceymfth.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3msrgocue.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cyzeldlc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3byfvlrfg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3pvgumgda.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3swwufdpe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ymlaabvf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3rnyvljlb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vpsvpjpw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eqgmbtjv.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3usudyvww.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3kgblnxvp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3puviygig.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lokmsfwn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xrclyjei.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qltndhie.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pucfncqi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3hxokjvvq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3sldhinuu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3juwjqqxa.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hflaxztx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fubvmwts.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nztremno.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zriswtxn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3hbbpexwr.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ppbcylaz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3iwgjhghd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mpspcxep.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3nngmvood.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jalzfvkc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bbkuepqx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3xnjzsjra.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3unrgcpzy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzqnvlq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xvwdqqli.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kstmdqje.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ypvhkqwt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rtovbldj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yhexivdu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epucnyvf.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3emnmvstj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3fpclzkzh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3niezulct.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bhopkzpu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3blpxqsxt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ifvfpicv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xuzekgew.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3fltvtsfk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jxpsbzpt.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kncijamt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3csnhcyas.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jstsmbau.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdfymhll.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3trkjootu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mpotocsy.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nicqpbbk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3slywqfiu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nstawyeu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lsngjfyl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lfiepjgy.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3olzxqihk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rniclxqu.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rntafpva.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbpmos.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ddtdebrf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwwmzbmd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3sdcbqrwy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3oemgnmjk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rwpvhhnt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xzlrpuai.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fkcdnkwa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3msvqhbol.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pewyjqss.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3owdfvpqy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3cxmbcfgu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3vjksdwxu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tycadrzl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bdnnwtlu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3reweywws.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nnmhpotp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tuohfwqq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rloyxbku.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mtnercvs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3sxzzenwi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3hhvgguwh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3baqsrzac.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3zoglbzee.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3msqxiaop.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3haabvwid.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rrxcvkux.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yzkuxbjg.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3awsnrdhw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wqrfezzf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pwdrivcm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lefntfgv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3zzusewjf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cfxabxps.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ujlgbcxz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qutncbnv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uwjxbqmr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hdqfzlbn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3uodwoofp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ibgegzvz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3eacsyaov.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aljieppx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tivrnmin.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3owwsvtcm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zeoxxjak.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ygyjhxxx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ixuisrqz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dmkmbpvw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ellwpbvr.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3biulxqlp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yjpwwdzc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3mrugvctx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zpgfujkw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sjrbcbrj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fyvialod.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ejilnywx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3mxsuftmu.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bmirhhgn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3yqdoxjmo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pevmxawz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zmfpinle.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dralootv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3zaponbkj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3uexusyie.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3daeajfrr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pjqhugsp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ccevqbqa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3faudinvg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cyrqsogr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kndhuhec.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvbdkae.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcamrjms.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3fgbndkxj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3sfwvruza.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sidugyqf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lbkcjnwa.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3dpjnmidc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xzoybkus.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhvbqjvi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vckgvzvq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tjcycnhd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jypehtyk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ufxuihvn.html


<!-- 参考信息 -->