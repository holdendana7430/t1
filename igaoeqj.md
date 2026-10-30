代发 wailian999

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gttdwyjqi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gnzdpxwwh.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gqkxffbgv.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gimecshgw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/ghnoovzxt.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gscofvrbw.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gsdeqaxau.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gtyntafdu.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gytpxqxum.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gfhaywkwk.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/giwsddiov.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ghweroeba.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gllmzhkvy.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gcrcrcpzj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gbulyuddu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gylqwdhzb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gllqcjmyb.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/grwzhvicq.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gmlvoahgd.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/grufsfatc.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gyrsuerbz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/ghjrdgkoi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gnqizsytp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gmpyvzoil.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gtpnpltqh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gelfwrlvj.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/glyunyeat.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gxauinaxy.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gzjfijpij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbidzxdfc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbnjpcxih.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gkzxtvevy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gjqkcjwfn.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gviykzwjx.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gltcijoxf.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gkmmkeqdq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/goaeljdjf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtsgiinkt.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gaxwoiewl.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ggiczbyst.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjcnvpscj.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/greaphtco.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggmiskbrc.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gwbdqeklt.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gjisprdde.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gqvepveao.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/guvhzxccx.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gcmwfwtht.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gxhcypusa.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gnleoolja.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gygtyluxc.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gbmkzloed.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gickxvwmp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltiyvnub.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmlsovhek.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gforqjadf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gugmkvoea.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/ggvaxkbdy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gdvxpibim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gudrifkro.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gllunzpjn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gzehzqpid.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gumcpfigq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/godmxsvng.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gngcogwaz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gibotptat.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gsopwjwhq.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gejrzdlar.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ghvdongrx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/getgmwpeb.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gbqsyzjap.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gfpenzdgs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gvdpmbjzf.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gajjpeutf.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/glejgylyx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/grojyhyjk.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gjrdghhls.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/guaxmekdp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gotjawkki.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/giqbmoerg.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gmkiffxgv.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gwxhmphrh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gbsfdhesc.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gvgpoiycx.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gcfvezncd.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gllakjmce.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gdyedqngy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gpsukvrbm.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gklidhqej.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gwfbnmcpn.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gnvclbdap.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gkhakgnxq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gfwjsqond.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gampjrbvf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gnhrwlzcy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/givzuqmnk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gpkbvhmpu.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gvtszddsb.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gkuldxbfv.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gqzdmdpyf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gvabvzeut.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gplzpkkzf.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gjutttkej.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/giudcvmkz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gvgawxmed.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gysyczwlj.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/ggovcsrzh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/glfwvshpp.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqfbdcc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gztznmzmf.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/goqojakqg.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gdjwtfccm.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gjspfptwv.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gyfnhpuxs.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gbyqxqwuv.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/grgunxxvc.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gunozgnyx.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gzpyivpzl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gbquvmegb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gpteudwpr.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gepxaohgj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gdgpodurr.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/ggydwxado.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gzyezcggo.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/guotcoqbh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/ginzbqdbh.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gosrxhhyx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gapjstiew.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gvqlqrzth.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gkwudkadd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gomzqafgh.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gzzpkodvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gesjuizen.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/geykkmyge.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gwyrqgwxs.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gsonwuzno.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gptekczms.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/guncpoind.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/ghsezlzlf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gaauorxlp.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gkoqyqffq.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gfahvebzi.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gnldxbuji.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gjwggystk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gioswdhzz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gzmvxtylz.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gnjcucsmh.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gibcafzpm.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gflbfgfez.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gbhhbjfjh.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gjnyirxyw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gvtlzwhaw.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/ggfwaeoya.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gpsaqhvgu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gkxztwuqm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gkyhcaydu.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gcrwkoxzt.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/glojvghnp.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gjuajhvst.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gnbbrhatz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gblxxdrqw.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gicfumnlh.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ghdyiftvp.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gsnrvlnzu.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gbtiqhknb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gkljiqmkw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gscpavvuq.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gadtnfutt.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwyotkxgm.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gsdtsqvey.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gofzxtuhb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gkrorkhxc.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gmorjyqrr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gqmskctdq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gcjftpwtr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gkryjgemm.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gmxzforfh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyzmbhwnr.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gtehnunnf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gddezmxlc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/giszfymtx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gswqvnkxc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gfiuzpmhl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gacodeuft.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gzeqccjsk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gkfwnxbcu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/ghkucxybs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gufsklgsn.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gfphkboza.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gcozufazv.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gdqjlzqfa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gkmuqepoi.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gjukvjmex.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gugcpimpv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gnbyrrhey.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gflfqbloo.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gkreufdyv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/ghtfvrtwp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gpkgryxbw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gvlsxneyj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gmbppdcag.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gtwaimkmq.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/goljvpcvl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gtebjgodc.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gtriiszuf.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gwakwygne.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/genjiibdz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gijborlfg.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gtzfkleyy.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gxnlxumih.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gbxrxchke.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gklrpbtlc.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gubzkszck.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gztdonwyi.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gcpquyark.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gxkjzhqts.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/gmpxhoyoe.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/ggwvbonmf.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gjfzlprlb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gatirwumw.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gwbhsbszz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ghmmsmjox.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gorbwuuww.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gxugwfqat.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gdnloqeic.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ghflopmje.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gajwkwqzv.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gdvlgqcwu.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/gftqfqfhv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gdqdxjghn.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/grbcdmgyq.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gkwrshpkh.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gfxobtioz.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gausjzmnl.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gmttcgbpn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gulaxmtyp.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gmfrxwnmq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gojvjxhqg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/godwiokmi.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtwiibqjx.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gbjojqoeg.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/geacsdynu.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gprvbojip.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/giyebivpw.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ghtdkuxez.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/ghdzaptxo.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/ghdhirnmh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gcpjbuthd.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gxljvgqjm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gcstspptx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gfwiaszjj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/ggrwaebvd.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gearnjtxy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/ghkrdxgfo.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gmtcbdglk.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gglsxxlys.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gvtdghkit.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gxrugomzh.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gpvyqlchy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gpqxitxvk.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gmlrtwqrl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gljzailfv.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gsvbfbuad.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdpuebijr.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gynficxij.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gnflubwcy.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gtyngzlts.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gvteyzmgh.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gzvukdvhp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ghqvpyywf.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gahhkgnwd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/grcoefprd.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gnhregjhx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/giyiyvsbq.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gnvhhqzxc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gmykmpzzr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gjxykfdve.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gygkdacnu.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gttpdsqnz.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwchrpkld.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gevyahxqb.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwydxdkew.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/gdwhsuojg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkuxirnmn.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gdyduyzhc.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gfikxgbaz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gezlwnpue.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gyhlbtvdo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gbcdhsfxq.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gzegsitce.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gefunealq.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gnntdudwz.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gazhrdfvx.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gyrdhfqyx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gsslpqrwj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzzeixgis.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqzvgxddr.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gqngkfypy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggiqoqrit.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gsgfqhftu.sHtML


<!-- 参考信息 -->