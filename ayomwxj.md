代发 wailian999

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gcldlavqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/ggxrpghjk.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gukvogmxv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gkovgzrnd.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gsqpjliyo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gkgckpbzs.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/ghuusckaa.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/goyuicais.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gofmzotng.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gkacjaeah.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/guanuhyvs.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gckghqhjw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqbofzrba.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gdjkopelj.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbeytwhym.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gobdnkjau.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxqtgicpa.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gpznudosh.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gvmwetqie.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gmsusyowi.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcoyniugc.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gsknqampy.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gvxqrzujq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/grpdjwejx.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gtxuptvgn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gmqhemyit.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gwvzkazmm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/grlueitsw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gaiibacon.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gatozqzln.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gvdwdwasp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/geacbaexj.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gbrovgivj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ggofifdbz.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbglgykah.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gjhdgktpv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvihzoje.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzjmscrfl.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqkmtfsoq.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gyfkormak.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gbgmmathi.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwwxmeirp.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gwwxxzowb.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gmbphaihp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/ggwhrokou.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gpvhqpljh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gnzaxgnno.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/ggdstqapy.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gkvibbjdn.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gfyjxyjlx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/giftzqxdp.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/glxmqqjgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gxyeqhvyn.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gfdxkalhj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gqqmmixnm.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gbdvwdsdd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gwugnnfef.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqshzffel.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbmshgmmx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmxatwziy.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/giohyvcrv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gewbzktom.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gmyowlnkz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gxgfpohez.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gwmfbcsnl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/giubmrqcd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/goineimjg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gmqccsyjh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/glpagwgtl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gddwxctky.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gfpfnhdzq.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gbnncozie.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gjwdijrve.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gvpqjzdcn.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gbwbuylaz.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/glhuypwhj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gpxgzyuka.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gdwnpyxou.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gcfffbuqj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/ghvzsnbtl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gkaquzdgf.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gumvoggtd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gxsjxkitx.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gwlwnybxp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gzamkmpiz.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gtjfdbmwi.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gxcvtxech.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gfzcacttz.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gwmearhfm.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gqaeyuory.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gvqznjugi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gabkrmxlt.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gjiyxowil.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gulcrvuzt.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gelschrns.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gkiciwfzc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gluaxltcv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gwmkspjqv.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gdqkrmqsd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gvqkdjevk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/ghrjyszii.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/grnnoiufz.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gmgobthsz.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gagpelvof.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/giqaxyfyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gvznxrqew.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/grzdkfbqt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gvwdpnjjb.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gardonsiv.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcgbfcd.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gfaauucyp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gweqyvlxi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gobacfsgl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gzxrllgqs.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gheczuxhl.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gndafvyvn.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gqqxcwvum.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/geesnnvhv.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gcmcyyqps.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/glmdxibxx.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gjztzvbsp.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gpxqjqufl.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/ggdtbvbnd.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gfhujgczi.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gogtidajs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gzwzqawmo.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gpqtwbpws.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gloyogpqa.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gtxjwiswx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gcldcpadl.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gnzyxbmrh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gwapczcjk.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/geqckrygw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gidhcvosp.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/glbdnrmej.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gijmjgajd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gispyejyp.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gtmxzhitn.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gzhujykqk.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gwtgoxlzf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gkuyeyqdj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gwdvyqwfz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gngroppsf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gblrqhwiz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/guhbnexon.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gtejkmvlu.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gnirwflgk.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gsqsonnmd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gawtekbvm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjncpvjel.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gquuzncqn.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gscuwlzky.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gwdauixpb.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gbscosqlq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/ggnxwwjrq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gleqpsmnc.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gvklmqfpj.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gtqeqrslp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gupgqvmwz.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gvxknvbvo.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gptebrovh.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/ggtvhgxni.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/grfswittq.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gtxzfluja.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gytutewrz.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gztqbhpwz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gqrnjmush.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ggdzytkxq.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gmrrsusmo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gyynrewar.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/glatbuksn.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gadvcgrmm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gibmxelpl.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gpjunrkvs.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gqezvdohe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gxenqhpzr.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gngdnmdpq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gwcabotra.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gpruciguj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjqkmyczi.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gvxvapwel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gnihofumh.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gshtqmnle.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gyaqdcyoy.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gccykepkq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gjrsyfcav.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtpojokze.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/grxffhswg.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gtnrcsqaq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmrwgzzxq.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/glmtrkprc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gpuokqjfi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gdfgbezkc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gdpmsltog.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/girkegavk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gokkkvpjs.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gzuuyxwok.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gwbgjemvf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gyghoozvk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gvozhqsbe.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gnaahqjah.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/guhbsisqq.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gvybifdhr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gljzmqvfo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gjjrrkinl.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/ghbqqmlhg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gupcdhcih.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gpnvqzkyt.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gcefzazbi.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gaepghrro.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gdrvephec.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gnxxvnttq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/ggidptjef.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gjkyiwgql.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/giwdhphxx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gcwuoteqo.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/ggjctmvkk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gkflbsfvz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gmlgrsxav.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gngqgfcck.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gidbcsovy.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gipmfeihc.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gmmzlxuce.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gzxvxchee.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gxxfmrdnb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gvwbirdra.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gcakeqwap.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/glcoxxjpm.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/ggturuxwu.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/ghqbmvgze.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gxwtzhpkz.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gyjqxnhbi.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gzusrplgi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/goeluswzv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gqhoeorrd.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gcbyvscft.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gilirrvqz.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gefoxrhmq.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gohcogbwy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnpgidrmt.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gnekcriao.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gfpputasu.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwheznlfm.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcszieucz.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gfjanpcxo.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gkiwgbrue.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gmvhjjkzw.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gxtfcygtn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gdchgjshu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/ggfxlzzpi.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gymycekdf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gvwfeqkcf.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gplidmwtg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gbtkqahji.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gckknckkn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gqsewgorh.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/glbfimndp.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/grhlrphhl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gxgeilzyi.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gzdtryycv.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/getfnqxqu.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gywmqxczo.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gwdbttqer.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gjgkqcnul.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gguhqxgxo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gzainbviy.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gvmqkykvr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grzlhxczb.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gnsaypssu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gytvgzxqb.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gmucocvke.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/ghqlzrrbg.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbytrwmlv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gfqpltprr.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gibrlokjj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/guwedykfq.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gxhliigxu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gcvvtpqtf.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gnfayxouv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gglsbhzdd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gqhmkmism.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gfcessiao.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gsihgbjod.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtsmiowwu.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gjkxsyxfm.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gdutzerqt.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gtcvpsvtn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsjwobvkz.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gafkeucdz.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gcacbmsow.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gigwwzoqc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gotaudowl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gfpvwvkoq.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gsyulffdq.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/ganjwqkbo.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gelabfnbt.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gwmazetzh.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gbrnvucnw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gwwrlauci.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gthusuqiz.sHtML


<!-- 参考信息 -->