代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqlbfpzj.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/grpomekwp.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyclbeakr.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gysgvixel.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhlfphc.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gstnrimck.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/grljifacj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gplwevnco.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkmwllrym.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvdkuosd.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gttyhmyhg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gdfpbqhps.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkdqhydao.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gnhzqmbmj.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtlstsjy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gixowlilp.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gtnqmwico.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtrxshqp.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxgxdhuz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsmtcwwrn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjjibkz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpynceatl.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gctczlxch.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfknqrft.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gelfyacsr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcbiavy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjabmcuuk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/ghyqofihh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxkfwfljk.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcdchjkgk.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gajqerpef.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhkqznp.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gegkmzyat.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glzpfzpgc.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gplsylopf.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gysscbcgh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvpazaft.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gtgbqbpqd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gguizgpie.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gxhzgsgyx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxroffgvj.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gcjlvnwbv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdzrzbrv.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmefnrwsd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gstvkpvxz.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gpiesqcyh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzfbxrx.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqfesxyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gmoawsvss.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhyanhom.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyksyxgrp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxdwhqsj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/glwxgafbu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovukfjw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbyjdnba.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulzfmaya.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gqzapwnfb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godasrpyd.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegyxjiqp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxirwwlr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gbriopvdj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gvikewuqm.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gcdhliijm.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gepvccpam.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gjzczujnk.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gosarzygy.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/glenhkewx.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gbskrwiya.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gnncanqze.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfnjeyac.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/ggucuxxxh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/geecwdrbz.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtzxniryf.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gzyauzfcv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gojqrroel.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gkcgtpsvk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjitluzec.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gllnmttoa.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxrdqudat.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/goacwkwkx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/guzhpgldg.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/goorohrlx.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gcqhcwwuf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecgugmup.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gggkimkuo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gunjlnbqp.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gxbmrbtsk.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpihswfew.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvoxrwql.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/geghvlecg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gfbbycdmt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuejmddd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezyqjybo.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gtudfflec.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmdmdcbi.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gadrznwmy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntuifeun.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjcvzytu.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gtrhdsxvp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqzuumuo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdcnxnio.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfttamuc.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gefjeedox.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpqskatu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gurpqlyua.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gptztdkmp.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gtihmkttm.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqlwahjz.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqoehejc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gogvcofco.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gfixlkqtu.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcsccwmi.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/glqomeute.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gnjyxedmx.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggidphmsz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gglizqhvj.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ginhbiojk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrhqokdx.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdvsyat.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gjokrvtmc.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gkydgpwuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/gpkeyszgt.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gmhntypme.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxvqdham.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/grjeywlem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gefhresqm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gmuguczru.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gdeahmuod.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gbrzekicf.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmandplz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgbblrys.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvpsthvh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gspclwoab.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/glnqdvyni.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkcxsncj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcejeysbr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gryumzggj.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gtvihnbil.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/goerhpkrn.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gvjezqsex.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnglxac.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gurmxjjmj.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gswxyfyyf.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gyhjluwpd.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/grhwicbxg.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/glpbgjtre.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmgqryrn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhkmeoic.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gyaefoaah.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvhtexnt.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfocqrqt.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glqvawoie.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gngaydlse.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmctrgkxv.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghczpduxy.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gavalsbrl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphaoawwt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqmhsar.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhsrauvs.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdvqycup.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxjirufg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzlysmw.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqunrcrgm.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnrimjqk.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgnlgbuf.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgchjrhr.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gyuamiadn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylwwmgg.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gocrqtjiv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqdzhckq.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gttqpcacw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gbhbythru.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gmgfzlkwc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsimznbja.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gfbqcklai.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/ghkwkyled.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gkmmiihji.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gofmjpveb.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gixhlmare.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifmtlvvj.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzcmpljd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gvvgcnyao.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/grrrpgygi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdcixrrj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gehugjenu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwdrujrm.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgiffsdt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkirilfk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkfptips.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumuueksa.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcivclrwa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmftndlk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkvqychj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqtuejoc.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gsxirbtxw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/ghfquxgkr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjrzydug.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gazwdhpyc.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpunqjdl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwtgbgpn.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdgbinlz.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvyfggwk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwpmpbgg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkxhdxgq.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gajexwova.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gcamaxbyl.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gghvpvfgu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gazjxlreh.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gvwtkkiji.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gikqwjnwf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhjanznc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gdlnlolcq.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/giuppratp.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnrvxayl.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gdczivejd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecxpnsns.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gtzgvmhma.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gurhyqfer.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/grmrbdxsx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpnkbtux.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/guvfpvndg.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gyngbmlgm.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gjevewrwo.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groisrefc.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/grljggewy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/grgcvifcc.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfbkrisp.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuwyjrtb.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gtkimncxk.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuxxouae.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvaplcje.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuxtsfng.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdvlyrx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gaorzssqk.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnssdniyb.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvyjnacbd.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhkkorkg.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/grabmnbbt.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjynusvus.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gifpbfsmi.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozwnztjk.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwkzgekd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqehqhrex.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnuejjjjh.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjxlqzx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmsgipmf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/guavdiwag.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoymrukr.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdzfxaws.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsumooyon.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gkucalidd.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gdigsbpdf.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqjkeyaw.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gpcrfelxc.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gckwfbvkv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxhugzkd.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gvyqnwsck.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gktvuvutd.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxuctnxe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyhlebli.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gpxpqkamu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godjxwwlh.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmldykhxh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gyweawxlp.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/guexpfkgs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gajjsczmk.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gazwvekbc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gpuamjnge.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/giivnwxnm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsworkyw.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyiktbek.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gxkdumare.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhcmmtjn.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkpsxyru.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxktchh.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gurbkjtpy.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbjedygg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnacieij.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvursowc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqlnqeeq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkhrqalp.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlbmutdw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gsvrnrgpu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghuxdnsvu.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gdpdajnhb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/geaqxzlmb.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcgxbrea.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gqyiudkpr.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyymiakw.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjtkwwxo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/guoxvqcjo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gpuyraida.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxpqvaugn.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gisxxouqa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtugohop.sHtML

按语言统计（条）：
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeodrhpo.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzzzzfsp.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrkvchaz.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmyshho.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gkultyffs.sHtML


<!-- 参考信息 -->