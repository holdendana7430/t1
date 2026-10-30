代发 wailian999

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gfapzxczs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/ghbotharz.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gsgruepbe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gjighhtdd.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gdwybyuux.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gpknhbkou.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnktnjiet.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/givzihyrc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/glqcofdzj.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gwhkhsowp.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gqnssmrct.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gtsqhxqqy.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpwoqaivg.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gzfebzvgs.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gaoxbesaz.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gxugeopuj.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gfiuzqdol.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gegqgtngq.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gjuggtyli.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgfjdyh.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwhtxicyg.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gknciwhns.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gpwlxuaju.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gdsidofqe.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/goytespmg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gafqdaezo.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gwfbfhusl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gbsubqobd.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gozubnihz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gkylwyetj.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gjbxyrhot.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gvoagjdmn.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gqkyhzlal.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gumuxccej.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gayxzuqcy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gjwenjbsn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkyvwaxv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gvkemwphu.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmuehstuq.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ghkdkqynb.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gkfhyprla.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gtuxxukrr.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gprycxtwk.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggdngcmqg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gyovhiuwu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/giwnwdhxx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/geazykaxh.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gxijjffgw.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gamxyyywa.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gdgbausez.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gteuogtli.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/guqyfowzr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gmikagmvx.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gxophnfqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gkdbtmiyg.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/goksosvcp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/givrxzskr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcxnmghtz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gfynpwgws.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gohlhdhkb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gfpqidwoh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gnwhuvgxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gkzyhhtfl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/grdazheqa.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/ggvsskkuh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gvkybeywf.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/grknftydm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gfhieutvw.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/ginfktlpb.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gofrozxte.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/ghflgvzxb.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gdndcioul.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/geyxvpviy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gjkpvutww.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gioiyrfmq.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gjfjkovwy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/golntbjrk.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gmhnpputf.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gqqfqharm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gxsglquxt.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gsnkyixhk.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gyisgljex.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gpegtqoan.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/ghmindmmd.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gphwgqkrv.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gsykvhdvy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gfzwxedxl.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gwmhhgfcj.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gnsdwfxan.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gqmbtmvnd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gwxrgkcjw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gbetkcjiz.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gfjlsivst.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gdocenjbe.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/grrobivqs.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gwwsngkmq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gmukboakf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gxkdhqvmj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gouywestt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gltkvaabq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/ggwvojgxx.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gmxdbcjqd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gtprgzpof.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/grabvuckn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gikhageto.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gkuxjtxwd.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gjoqhazbw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gzyuvjwzg.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzjyevxqt.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gfloiilwr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gmrblxmig.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gutpparis.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gxpmxqbln.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwigirddt.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/geohdcuig.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gkqimbkeq.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gqwwfgact.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gttqmnpcy.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gsziaendf.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gojbxbvgk.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gdtbzkwln.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gnvdlidkt.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gmdcxxlbt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gduzpgdfd.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gsbvvqcxa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/glcanjxei.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gnvgbsgti.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gdzpezxfn.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gihomitoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gloisrrdd.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gddydmxbo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/guhniddrr.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gzcpveqfz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gasgcdcbv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gvyroljui.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gmzrwuhrv.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gahjcahsv.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/grrnxsmvg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gguhkojix.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gnqywhvrm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gmyqwcpju.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gbtauintv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gagsjrwaa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gbevaxkhw.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gdtvfteki.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gfijcoqwe.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gudmxzenq.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/ghhabckck.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gydxvvzqj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gldjlzdem.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gxnglbwkf.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gcurvpnyb.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/geflnscrx.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gjuriyfxr.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gasdpbkyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gqyygqdex.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gzbpxhixi.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gjissfcrf.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gpasnptvk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggxumvibt.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gxhdtkrgw.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gsypvnbio.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gmzctfbqm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gfiwysmqk.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gffwuoiej.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gnpnmuqdb.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gjajghepo.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gmsxzynwn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gvmdouyub.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gorlkvluj.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gsxyhsgmv.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gawtiqtua.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gvjpjvxvn.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gaivsygiu.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gymzqyekk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gatercjki.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gbzvdgsql.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gcjrqpnkt.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gctfhahtu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gdhrcdmsu.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/guiyblnuj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gipduazow.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzvdrderx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gxczuwzsa.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbggohnpo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/ginoytjta.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gzvlcfxje.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gjsvzwxwn.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gxjgigkiv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gyehqmtml.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gxjeidpbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gzlzcjfqb.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gjfwutqtg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gvsqknhlk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/grfmxrwdl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/goyucxgsm.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gynvbkacn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gnqsfaaew.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/goicxbzom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gfcwyuadr.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/ggsyzzzmn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gerseqxnu.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gngqnkfyi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gagdtukxg.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gibrowdhg.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gopyiwrel.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gneqprjud.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/ggtevyllx.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gpfkgkvqi.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gavypitlk.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gtemrvvnv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gzysvhaoj.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gfowlwjrm.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gmcaaiway.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gkpswyexj.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gorkamygo.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/guwfbckju.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gftrlbgax.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/glyhpdcqu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/glaunayai.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gjsmqvzco.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gnorydgfm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gjbzjerki.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gudfpqikm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/goybbiuob.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/grdtfcumh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/ghjodvrzr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gwhfkujyl.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gbslzhyfr.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gxeyxprpn.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gnrvywqtv.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gbzcfpdtf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gzewdajmh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gwjhfeark.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gpfoirhyp.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/giyxabcxp.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gpkfjahnp.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gwytjbdnz.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gkoeaxxth.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gpxgdlxvw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gaqexmdvj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gotsjuqlr.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/greszlazo.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpkcbsovq.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/garcnkemj.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gmrpydwyv.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ggzwupcaz.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/grdwwamju.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gzqcttcib.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gzjbntqgs.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gezyeqztw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gbddxnfnd.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gvnziqtsx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gyuxiefpa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gfjmmcjhn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ggdjxqlml.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gsblmjdrm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gzcymycoo.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gffsdwccu.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/grqwgfvrj.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/grcdkvmxu.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gvapzfffl.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gnjqwcsmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gxmxxypky.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gmiefmxhy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gqzxpegip.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gnaobegkh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gbtlzabmp.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gygzsewah.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/glcxysvnx.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gmrscjavp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gyqgbcirw.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gtaiumdhy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gqeujdose.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/greybrxsh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gbgftypqw.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gdcqwdnzv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gyhcupwrv.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/ggiomoylt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gykiuoctj.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gbevoxvef.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gbdxehllo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gvdfjqprg.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gfvrsvhqd.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gmcejjpya.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/glxxborrk.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/grzxyyzqs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gxfciyrtu.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gjxhtqads.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gjtgvijes.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/guryplirz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gurfvvemr.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gfkjmjars.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gprjbstvs.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gdhjuphpn.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gpurelosf.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gmftgpjkh.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gudnqogeu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gvlcqrtzg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gglqgqrzc.sHtML


<!-- 参考信息 -->