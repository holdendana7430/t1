代发 wailian999

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gkczpntqt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudycvxdj.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopytkqjm.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gaxqbfjvv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpeiexut.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gkyhttpsg.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfrwnsrrt.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsomvnuyb.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkwednzte.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gugfensbg.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gbwrxzeug.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gppspgfjl.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkigbllii.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbltufulg.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpfgfrvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtawtvyt.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gptecwola.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/ggrlgplei.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxcrynil.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbudkxyun.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gawzvbzvj.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gohvvsygm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcncbmknu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmrbpfnib.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpofsdkgc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gntowmvkr.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gscipebdq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gdztijulc.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnpowgdbw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdgfycbs.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbugtrtgx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gieekswqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/grhbrsttd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkqrictk.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/goptljnbt.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxnovaib.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkukixaz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvsrgfvr.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzpsvxp.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gohjbzfqs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gavudoqej.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwrktsjn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/golgjldez.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgdygzav.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gciwxlrtu.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbypvwvp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjovwqe.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gyzopbhmt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpspvcd.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/glmowdqwj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfsnbpxb.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwtsupux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gprfqfbhd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmhwaveo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfalssqhc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqozejemk.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbwaxpwv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjijsqzeg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gmbdkgxpr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonjrcxio.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiqkazjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjizxjg.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gvdiugkrs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexhztfre.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkstafkd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grdmdtvdd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxztreobj.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvjtzqb.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/goakjyptu.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/ghsjmqxqy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gimusrxcf.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gkwicadgv.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gniaaylhx.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefxsbyjo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfitiauy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkvjruwr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gibvaodsq.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gydbxehfc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvuzlydd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/guqwhoiao.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdrcncim.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gkjtsgbsv.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbvedjdj.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gmwkrnvtf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftzokoip.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gcmrhftou.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gydjpsvwh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/goobvsabi.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyuwckqu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrdwtjoj.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gxznckrrm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/govqlrhea.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbzbgeuk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizxzaqql.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/golpddoyj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzmbmifp.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gumoaqtyq.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/ghswhosxa.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyufxzny.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/galpqcltv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxmnxhxgd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmqedzal.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvsicbvyt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzyzuuwi.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gkosbdcyd.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gljrsumyi.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqfqmcbo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtcfjzna.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxwtbilh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnznkdxln.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gdkkwdhkb.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gnbddmcii.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gqrcmobyc.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/glcukroru.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gdxyxtawe.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfulhoxsr.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/galyeeyxc.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoddavto.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyvrmifea.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gnurhclbs.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gxarodxot.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gkorpzkuh.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gvdcxncmy.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjbaytes.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gezdstqlg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokjdlyvq.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkfxuwqb.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfehjnlqf.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbamsswe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gkasldmac.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkivmeywf.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gwltwzjkt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gbtzyfbuf.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/glddhkxwa.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkijoxmi.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyvgnynt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/ggiixpytv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gjubtubpv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgxpovge.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/guyrpewcl.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvhgqwmk.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxyjmmpy.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzvnpqug.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grszpuoix.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcbdoighj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmfqjsys.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/giyohqkpk.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gtqrecckk.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvnpbvaq.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/glprxgoyr.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gohdqfpai.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcoafyk.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/giczkvasa.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/guhfceqaq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gyusbhwff.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gchillzrq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphclfqcy.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/ggbmsdzrk.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsubfqfog.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/grxuppbvu.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfjqghew.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gsiesxjxr.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gytzmxwxo.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gevnbswob.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gauwxsegk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gylqecjhr.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjroklpfz.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gosafdazd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndxlumg.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjfpcplv.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/grydiwwno.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gryjnajqf.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/gjqlbpmpp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcttctjto.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrtujjl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbolofws.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaicsixd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcelantpm.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjukekz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmrymzaw.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdvvlttb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/ghapxnblb.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gltcvkmpj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvehkcb.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjtxaokq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmzktaso.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycdlqywx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzdbpqvh.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gcabyxxxf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/geyelbxkd.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/glkyfxqml.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvafvmlmz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxrrdpvt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfxsxlbo.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjsdlgs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gzgytjxdw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdaouwexi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvwhzqsi.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkepkcmkl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/guxfutqnp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gvfuwijic.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gumhkyvhn.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdoportux.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvyexqj.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gjphhcgzr.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gdarssfba.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/glqxruhdz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/geeicjxly.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgdfwpzh.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gcnyzslxy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gozwdakut.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gymbnftqw.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/grlamfqcs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywcunohx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gaatmoaas.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gckwiymuh.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsuzvdfi.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhhcqdfb.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gsudcdzka.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjcmohku.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyjlevmn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggymyyrvx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gprtssdxq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzdeiwxg.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gqmonkaxh.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpccadkjq.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaslspouh.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhsveico.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzemtuasx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezasiquq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaieaywk.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gzqeytbvo.sHtML

[U89] JS：数组去重
来源：http://3g.fanxiaobao.xyz/Article/details/gjeycxqnp.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/glfctvwls.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gslggttma.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gybtplxuy.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gadxohwvh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gvbajvean.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsozcjdr.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsrpxyvb.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjzhrlh.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/ghchjahii.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gswrgwese.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmqsidft.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeowbvlk.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grrakwywp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoiiciir.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/grscrfnra.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebvzzsal.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvtspgfn.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gcvzfijxg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdjfmhzj.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/guokxxucu.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfciszef.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/getopgwma.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubhewxo.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gimchdkun.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/grlzznixj.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrgnvcei.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gjpbgurly.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiwionan.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glymgvljp.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkrojubm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gtpjeffur.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/ggkmoppec.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gadvsdsbi.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvwbljv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gkcmfjpgl.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gyeruljeu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gweqnexwh.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gpmcsyhtz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gshrxiolu.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gidbmgert.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjctjvzp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzockzkzm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdoatcjh.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwfoyhf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsssacsoc.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/glojkwpod.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gbzgkausn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gkffwqlen.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gklbxtrdd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gimhpiiha.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbrxoahe.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gngccxufd.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggscmjytn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvagwsrsi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcgphfzom.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbrbfezp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gikinrgxv.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcrdzhrh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqykqcvx.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gairounoj.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrzjkiqg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdswsnmo.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkgxbam.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gddkjvavy.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/ghwnwgcdj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goptojuty.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpbcyad.sHtML


<!-- 参考信息 -->