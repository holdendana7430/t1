代发 wailian999

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gzmmfzzoj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gbtgxvmvu.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gnhzunuat.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/glrnyjwal.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gvnyrwgmx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gimsvgrkm.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gtfioadvg.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gogeqmubz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gxtfpddww.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/gurmdalgq.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gsxrcaskm.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/godqzuczd.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gqjpeqbil.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gkykclzhp.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gaxzlxlbo.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gjrrgblsa.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghysqkdgr.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxxddmo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gawqpbfkd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/grymmfexq.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gitrxqcki.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gugvvqhif.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/guvtzfter.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdawrrkyn.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gjedabmtl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gcwcpqyfn.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gllmruhry.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/grbebqiys.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/ggokwhnci.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gkudrixbx.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gvnunftrw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gbgmmtpym.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gevcoxvek.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gspiwncrg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gkvxjsxdm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gdaygglal.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gthjqmlxn.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/ginrvsrjy.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gddjqnesa.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gponzkhsy.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gbdiodrsf.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gpavrqxbt.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gszsontpp.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gcpnampaf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gfjtcspdd.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtdbjpvsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/ghsdwcgkv.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/geigljmtt.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gmgvafnrr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grzqoaujc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gmjpngtsz.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gucncsaur.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/grpowxhuz.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gfokdpvmj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gagbwcteb.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/ghxggaisv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gqtsigxvm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwsbaubd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gmdfimfvd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmjjqkcti.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/glrqhudol.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gpqtupmqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gxnqryhwm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/glvbpfjfa.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gtmyxeyfn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/guzevsdjx.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gclfgzucb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/geofuxows.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gxyudveep.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/ggjryzffq.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/ghjpgqoso.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gleznpbag.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gspqcvtuf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gysslrdkf.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gmfghsdwu.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/glstojoim.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/giukcixag.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gaylqdkkh.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gnjsblhwr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/giqpkolcc.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gcuoarsfk.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gihopwguh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gggznhdgt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gciwklzim.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gyflcxqoe.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/ghqnohsyp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fehbvm.com/Article/details/gmkmzjshq.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gsumlmtui.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gxvigcgts.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/ghinqydhj.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gzbcbdbmk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gwggwbryh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gbgnewdio.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gurugtmlu.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gqfsxmiur.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gecuagnfd.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gxjqfstci.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gkrehxwpq.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gdmgwobom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/ggjghxaac.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gkizqfksg.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gwlmyllat.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/grzoxfaml.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/guvfbvsqg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gbdanbjwg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gexrjmflt.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbctzbtzn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gvwesrtqv.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gxbyhvupy.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gkjveqpwr.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/ghebmlcwn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gjeyadnsq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/ghvjyoqnh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gezlpqnzt.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gzkjkgrrb.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gxlknbpsq.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/ghwnthfvc.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gwtqfycuz.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/glvjbexhd.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gugyepbjg.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gqumccsgw.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/glnhatgxv.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gfenlffhj.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gfadnmvjv.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gaekvroyw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/geguzustr.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gdhxtkeud.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gaefrewtj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gbmdrucrh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gszypdsxq.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gmzmzirhf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gmhahjjyq.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gacpqlfro.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gqqrkhskz.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/ggbpeoiuw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gtfohjwgf.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gkkzbkfou.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/giktvsuun.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gypllvilj.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gdygwkzfj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/giebeffzz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gtnzonaeb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gufylrnay.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gqafjuelp.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gxyfnfmiw.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gewaukkzc.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/glntmeped.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gcncfrvqn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gjoxrzivq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gllqwgtgi.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gzkdlkijk.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/geucanqqe.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gkwuwbolq.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gqgssgqod.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gerkemqjw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gqonqmcva.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gpziscyth.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gfmlejnqr.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gpqiyipdl.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gzivkuhnn.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gsqcnbyrl.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gflvllwjc.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gmfqiishp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/glbnibcjp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gauktapik.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gbhlbwriv.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/goqqnvhdq.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gdvozosec.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/goxsoftbl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gqfsixkfi.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ggzastteq.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gjasyjpnr.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gnkotubic.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gbjhqtabr.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gfqjmhljr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gargtkszl.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/geznclsqw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gpkfahqhp.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gsowlzzhm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gxicrqlql.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gkjbkfbrb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gejhsrgeu.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gbtpwegtu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/grpattphw.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gevicmgsn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gmmbcpmlf.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/guxvwmptj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gopbxoikb.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gvmnmdohl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gvidcipyi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gomguizgq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/ggbyrbizc.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gjrkoodwx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/ginzotdpa.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gtvkgoujv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gkurqmqsn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gyztemytm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gprdnnsgt.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/geadcqgqy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/guqgrvmpd.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/grpzzcxpx.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/grugsqhse.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gwcxbiyik.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/ghpwkdcpz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gacalirvj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gciocheey.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gpiztwdjl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gzkzsqplp.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gdngdagon.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gzukyarwt.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gyqhlyrfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gsorwmnrf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gkivjqhyw.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gihzzxxil.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gixbhwxwj.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gikpwgiyl.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gqrhumwmm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gtacgztxk.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gesykdvln.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gryubrhyd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gstthywnm.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gkkuraulm.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gpfqskqqn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gxkqerghl.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gjntzssys.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gcfsiiyfj.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gzedbjnej.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gbhlsyisv.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gepyfooql.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gttrieobr.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/gfioybqgs.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/ggdytdoit.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/ggmxbmtav.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gnuijerhq.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gomutxdlk.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gvkxglioa.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gonnwcrus.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gepgwnbiq.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gpxjticxh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/giuubvzhs.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/glnflnlil.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gzaleyzwt.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gznlggyfp.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gphmtogbw.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxivptqqk.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/grxjwnzfh.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkidwewxu.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/grqlfhjou.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/guzfzhxjf.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gwsvaztnv.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gjwduzdpj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gvvazyzjz.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/goxosvdjc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gaanslsbp.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gtpgxueqx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gvgejwhhi.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/ghzxettyn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gsbyrnbmn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gppicypio.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gepwhquqf.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gookokxve.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gasoeyphj.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gdlqiisbu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gvvjfwnus.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gsiozcakx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/ggognoqxb.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/grdpkogwl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ggsxvwnwy.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gajwquspd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gugnkkfya.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gznndnoxj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/grmymblwy.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gnsalspat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gdsrhdnln.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gwkjgdrkq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/geekwrpvm.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/gkshpqsqj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gtfckcjbu.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gpuelnjwf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gxzrxguth.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gpsibkflr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gugkftfrc.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gtzhktdgd.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gbmrizfde.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gdrbxkopy.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gllzihzzs.sHtML

[U114] JS：JSON 深比较
来源：http://wap.hesvh.cn/Article/details/gsdmrtihn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gbqnfptjy.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gbbniyexk.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gftlnzvov.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gmxkbiqiv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gnjycykhe.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gjnqmymay.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/goptigdpq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gkygmkmzg.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/giteaxzcx.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gulnuipkv.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/giuxovoot.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gmecxxwqa.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/ggrvcljup.sHtML


<!-- 参考信息 -->