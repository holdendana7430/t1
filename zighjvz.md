代发 wailian999

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gtdpmcpwr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gtboocvag.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gllbblsmf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gcbxltevo.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gfsyuftiq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/geruwoisl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/goipxdedf.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gldkudvxs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/guizxilyv.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gplegsses.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gyqkdbwxp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gcpswkrmd.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gwmheiyqw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gcuvhdqmg.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gbpqjqpjp.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/ghegiecjj.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtbqfeavm.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gpnbwonrt.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gyivysmdf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gvwnhxioc.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gnsolvjdm.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gtfnaykgh.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gxjqdgqam.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gtokobley.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gjxlebaub.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gfkomsvfo.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gqysppach.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gzfbvxiuj.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gvgznekqs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/ggnvjfwxc.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gqnfhtywp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/geepahiew.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gabdmnjed.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiesxupc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/glcdwhaof.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/glmerssan.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gjsnquhoo.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gfbibkhjh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfdjudztf.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gdbtcihfm.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/ghhtrusdv.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/govvjpxen.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gyejkwhhh.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gnvmdxuah.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/grvphgwxx.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gnbcyezev.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gtznhtafv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/giqyizpia.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gblrjqxkq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gafivklgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gcqbmzcnl.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gwnyyijvp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gacpnziof.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/ghpnwvogb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gjuribzck.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gthbauoii.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gmuzzeebp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkgjchoig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/glzkkkrwa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gprhgvxya.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gfnrcydrl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/ghtvuuxts.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gyrdrvnfm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gfrzjyejx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/ggasstqli.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gyynizaei.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gawpxmwml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/ggktrmvtr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gruobpsaw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ggvhvwqra.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/grbfrbgcu.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gihjtxvbq.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gefwbsssr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/goohbvomb.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gtvvfdyyn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gjoxlqfme.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gpcltzeip.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/geyhntllj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/glajobfma.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gmhppkkko.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gksovqgjj.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmzefjlem.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gpzszfnlq.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/grebgauke.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gfxueghyk.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/guzwafjej.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ggwsubywh.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gakkznmsj.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gyecaapod.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gzylpqiqw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gkpsxmtev.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/ghxtfxrtt.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/goovyhdfn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gfdhnkvnt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gkmvfjfui.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gsxdooxtw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkfzjkw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gscraklme.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gxkkbundm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gyzwconiz.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gmilziokg.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gjzylyybt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/geqaqxxnr.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gixkvtknl.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ginbesthb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gqfspnvft.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gepcsfmpv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gfaxrtxjx.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gysywmnst.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gwtpmyjxk.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gngzbrvmb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/glkekjneh.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gsxglyivw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gcuxyvnij.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gswfzucdu.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gngknddpc.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/guimzaopc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gybhoayaf.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/ghmxgtthr.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/guxiatdvf.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gmizovaxc.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gjqdmsnfd.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gfqtpcgny.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gkfjzilkw.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gqlvgdudp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gmocrjjtx.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gelnnarqs.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gkmolfsvh.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/ggggsbnfh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gxodrduyc.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gxcmdgekd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gpuopiahl.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gfsefhycl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gaitohzns.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gqfxpkacs.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gmukxqcii.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gmvibtasi.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gvzogjuaq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gygnedjho.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqsafvqgq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gppyjnugk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gcdjcqevu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gnuwhpowt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gyxjqdsta.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/grzjrzwmg.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gwkeqsbxc.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdlppbffk.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gctjlogeh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gbgjpoqkp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxcvrwguq.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gjoflqwzz.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gdgsfymlw.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/geawkuqsj.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gcwpliext.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gqsgqyaqd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/ggesyvhpd.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gcnfryyuf.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gnyteoypw.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/goitgyshq.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gzcvqkjou.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/ghfwqkgtb.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gxhuwdfkt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gnwuizmin.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ggyxinrhd.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gpfbsrczd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/ggutfhvzt.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/ghvaixbpg.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/geakajaoe.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gwtzmwwuh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gmqmnkplc.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gkrmmacqr.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gtwjgulcd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gacztylcj.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gqkcmzayy.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gmliyjlcy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwzlcvhl.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/grprzicvt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gowyudhfc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gvmdeibjh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxzertvrv.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gndewdyvb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gxdxmlzzm.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gfmqboebk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/ghasxlghf.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gnqqtkzny.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gahrvngxh.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gqwvxtvit.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gxzhvijpk.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gjnuizogc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvenkumtx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gepcanski.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gpooxkrtb.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/ggrjgwvrb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gotirusgi.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gbbothtzf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gplknunex.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gubpipaig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/glsarwulz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gbfygprwd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gmmuqnkvj.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gpvorednq.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvkfhqnwq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gbfvczslm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/goijrqkln.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gxuouhbzp.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gnkfzfckg.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gogejtvet.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gowltaggu.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gfrxppttj.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gplzpjsde.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gwwaizhac.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gszhfhryw.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gxsojdecm.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gslcvsysg.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/guswizsqg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gwoyjsxwz.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/giqsapebk.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gbzpnykni.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gyzzijiuc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gyfcufxcn.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gcfcjhjqa.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gpzjigoyn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/grmuyncqj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gclehihib.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gpgziepnq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gjxklmcph.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gjfdpgxfo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/grzbjczxq.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gvtzlkcwd.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gcvjmvmnv.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gauubrhar.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gsbqskbvp.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gkguotztw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gzihmiknx.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gjtijtjzc.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gjdwgaxit.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gntglujvp.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxnlwelvb.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggnagnkyp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvzizetyz.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gmhdjknxp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gaifywhnl.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gxcsrvxiv.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdlxhbvkf.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gdildcbzd.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gglhehgze.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gmmwnugcq.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gunczvqev.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gwlntfodh.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gclqkjacs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/goqrtqlqo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gfvvbcwiz.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gmxtwslee.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gsqcxdlom.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gghhwlxte.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/ghvnkpbgj.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gludylmci.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gnlnbobrv.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gbkvtdslx.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gptasuxdd.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gcfkqvzbv.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gzbjaciqx.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/glibvtzmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/ghvcblfds.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gtmpnhjao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fehbvm.com/Article/details/govxzogml.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gvaztptzi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gouaxzmxr.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gginnqmif.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gadgesokm.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gmmgyoybm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gtsgayvfi.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gscfcibtm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyzqjovta.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gvmsbzjgz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gkfvxftwa.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gpgpfhkus.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/guicqgjax.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gejbxeeli.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gkpdxabqn.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gwkvvbstt.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/geodhwqee.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gdzljbijj.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gdrhsjkup.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gcqjiahko.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/grqegqaoy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gtbamhcrj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/govuqenar.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/glkkbzzza.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggircnhdg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/guulvkvmu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gflxzmrqd.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/glapiaqxs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gnlqumwre.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gjhhxuxph.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gwjcthjpc.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gufotbljn.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gstokfdlz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gdaomqtng.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gexrtppev.sHtML


<!-- 参考信息 -->