代发 wailian999

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gekbmhlxs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gyzvpohuu.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gwerlygsw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrxgnwql.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gvtnolcap.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqezewdki.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaaifcuk.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gyzxljzyx.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabogeaqr.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/geddfgmux.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/grtrpwdsh.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gprhzvvdy.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghgisrkpi.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaavavcya.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoxjjhbm.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgydbcys.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmanvefs.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ggmwonpvf.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gutllhclq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/grlocffcc.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxqxrwan.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gjrqbghip.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqwzwflur.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqqniiwpt.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gqjsitldy.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfzhmperc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmaejrt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxxlibwkm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gescoiiml.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqysvlca.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gamowzbrr.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gpktwompq.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuhazoyo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsktvvxkg.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/galgeeizh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gerjrhkfq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhyvidcv.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giwxbzxuy.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glvchbkce.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwgctogb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdqkhkps.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gktchzfwf.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gckxeprab.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gsktmsxzv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwaktymn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsunqka.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glothmjcc.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaomdozl.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwihocbto.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ghktvpwhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/glybmixjf.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/grcdnnqqa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtylfsxw.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gncdscazi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyppjdpnm.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gqzgndphu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gztvdnkby.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gciwgbtun.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqvwlmjh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsbwaqu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusidyxr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfdlsezb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gccodjlil.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgkucagg.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gejsoqkby.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gghtaanmc.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gsgdzqric.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/ghxfeookb.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gdkbrciwx.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gxckzhjhh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggydbihah.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqekbdocg.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrhphybr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gwgdhzssr.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdfaxbfb.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsveladt.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/grylkwazr.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojorzcee.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gnlhaycpx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gqmrshvnb.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghmtpyvdj.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ghuyajfnk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtzrymad.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqlcivqr.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqhuefim.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyalktxkw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtbifmfqq.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuyofleb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnfayjtx.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcktrldvm.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsgwvrkz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwlraffjj.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsaixvem.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/greoyiwwa.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjgutvj.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/geoulelce.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gogqmztsv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmqwyhci.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaiprnns.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gxomfwfuq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gflgzzljv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzltpxocq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqljccmrm.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gacxcaacp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsehdrny.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gawmmxnti.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtjliwn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gxomcxggi.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gbivqrwnc.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyitglcqd.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrjzdwxj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwbcofyi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gashopcyv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gwwnhlacb.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gqpdzhjzm.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gkxqvfbut.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoycitwh.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkjtlnke.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gypmnvakp.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gwzysxhpm.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzirjwygv.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/geppvfsbd.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/grqupptxv.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcduxuyl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlieibgi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/ggowtnnzh.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfosxtjps.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbpybvpn.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gmmkuofzs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpduojbaw.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaikweoyw.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gctngpcfm.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gjlehyppa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgvvkzho.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gvfsgplcq.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbtbjidt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gyhmsucxi.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gfuhqlwsx.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grttwvgux.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwnrssgx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/grxbxrnml.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuvtrlfj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvdftrl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaannvisd.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstddqwsc.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvztgme.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gecyspori.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvixlxckj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzihgkdhs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvojqgieg.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhendaus.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/glwqnapxe.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/glhzolmgn.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gvkcqirwt.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gjdzffmnk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggggbhtjy.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/ghvusivur.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/ggrarjbix.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gptjnzdea.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gigyeusio.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gykrnmyyp.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpbgmaps.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbvcqutqr.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/guvfeyhae.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbwnkihr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gjaivfrfj.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowvfcbs.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gptgwcstq.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gmbffzzcg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhrbfdxk.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpjbceqp.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmobsixu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gygtdlmjt.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwyztjvkd.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gtbnppnkn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkeksti.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqanbjvqc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gskictigb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/givegbopa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gisnesckr.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmfnhqmpn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhkmgki.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/grszxakda.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gdyhqpatb.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/ggrkyshag.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gpngpcehv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubnefcga.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gacfwhqcj.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlnfsiji.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glrliztpb.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gvetytdyq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvjmhpb.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gqbbercrm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbinhcvly.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gczrcjice.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrqbckox.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaualjqr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqjxwgl.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdcqprdqe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzubykyl.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmhkcidh.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhpeegy.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnafiigho.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gxhgqixdb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuwiomqc.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhttpggr.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrbqztsn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqhphzu.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/glbwzbwpa.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatfhzsxr.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gzumudrkj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnpnbim.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggczhftwl.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrsojvso.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gejxvqkkb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdoyqke.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhdycrkb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjzfgjtf.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjqrkdlz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiiybaxh.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gkjkzqarf.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/giqzbpqfv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gknwokvlz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnglexicg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxldnlxl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gwaipycmx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gysdhhlqm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqdofkp.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gvellbqjg.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjecivqi.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvsrbuqi.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpvkdpno.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsflpusxr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkydlnurx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjhwvoz.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaheoqez.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrbdsknm.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gwcxyjoad.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpmbethv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gddsktkbo.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaucsxmd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/genxbtfvf.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gaueojpue.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gshgshpgv.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqyhmlk.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulzrdcfb.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gujqdbrxo.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/goteeinjn.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gcvwnkomc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gewokcrzc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gvliwetvj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxuuxyby.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gwcbgykdn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdtzvbuc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzizwrtwf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyoaqhnv.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gfziolqnu.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gqezskkyr.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeitihye.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/ghijdrbmo.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/ggfkfvnxi.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhulzooc.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gipyuypsx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopxnoxsn.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwolkbn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwwtxccw.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gsubauczz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtusbmwlg.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/guurwnjnr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/girhddxtf.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/geqlqgcsw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gflijzmkl.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gaofacllg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymqrcjsz.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gznhniuij.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gzieysspe.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/glsswzbbd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbehdaihu.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtygmiqhj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyglzrfgg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzczmuwvj.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gyvbuvmha.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkpquhkf.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/giozhkndc.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvqcekx.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/grozigwpj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/guvwzusxz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmazbmnxj.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gpjjzafgo.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gnwdzegac.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gitoaafka.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmmbcgnk.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gylldemrg.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gqupqiayz.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzekcrjr.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjtixjsn.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnvewkam.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqheqjsk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcodlwiry.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gdmftiaoi.sHtML


<!-- 参考信息 -->