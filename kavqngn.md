代发 wailian999

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gwacofdtw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gqbeglriv.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxxtlutpq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gbhjtzqdr.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gljgrvdma.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/ghjqmsmfi.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gkaeoiort.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gexezfkvr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ginkxhawd.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/givfruzwr.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/geetkkepy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gaxorpftk.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gdqihuabx.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/grpuclkkl.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gvuilssii.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gnybjzqog.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gazrwwdql.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/goopzpbcs.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gacfchnit.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/grssrkwxy.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzeplmgfp.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gyuagbwgf.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gzpymazrx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gbvtksrny.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/ghvaepglq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/geebrewuv.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gtfugrllb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gmuqxyreo.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gbzoydttl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gzxvbmywc.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gjmmfwlye.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gzqunjyge.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gtcrkzmfb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/grirotziv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gvchsaliv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gzfusjrgr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/grkqiaapc.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggtfoslzl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtqgwvjvb.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmwscldwd.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/grslizayz.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdwuttieu.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gahabuxen.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gjthsadwy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gbzdybkbx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwptowrsu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gjjuzbzbr.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/glguzyeev.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gvsfcoodr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gtgspdynh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/glcycwciy.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/goolnpzwq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gonjrnvig.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpdwvcrdu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gebsqosvy.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gjurkmaua.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/ggwirrjuj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzqnluvcn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gknucehxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaheipguh.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gxteeiilp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gdnoevtnj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gzavbbjbo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gbunovyqd.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gsvvyiopo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gkyidpexw.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gnsbdcuhw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gyiisbvwt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gnijcoztc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ginnugxtl.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gokaipksp.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gcifzucid.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gqrwlwwqc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gzauryzep.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gofnpwbxc.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/ghalommbj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gengefmkj.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gfpbhemdr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gfljyfuwf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gaogzxzul.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ghndwivwg.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gkxsgunsm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gwmokpprt.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gggiohqzp.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gmuxnshoj.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gczyqzkub.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/grprljdxw.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gtimwacwj.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gzrvhbzzk.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gnegqdwfn.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gelkmfbuc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gpdyeeioh.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gfyflpair.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gthnxrfkl.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/glpqyfmlx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/giiyvdxzn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gulotkmbs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gjndxwayq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/grnmhdwnf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gerznhdxf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/glpojioqg.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/glbcbatxm.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gptnvtfdv.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gaowvytjp.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/giytqsdjs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gzpvvinhy.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gnazgydui.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gylpuxnlw.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/ggefsvrch.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gwcnhneaq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gdixpxzln.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gmtgffebj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gandluzdy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/glibqbopb.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gulymxujs.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gikhonwtl.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gdvtuwpcd.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gvmfipxbe.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/ghjjorqmh.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gacfzwrtc.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gzestrzdg.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gfbptlvns.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gatnzhkae.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gchkvxaii.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gammgaliz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gbxnsppis.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gbzjjtebn.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gcgwejrrg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gfukbyqbi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gotqqztaf.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gqufrrszb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gfzxdiaef.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/geipnjklh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gdpqxeohd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gvblvckco.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gkczqolft.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gohkxzwbe.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/grzwmwxnc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gpntbciiu.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gclmyqovx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gjznqscxo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gbhtyshxc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gcgbgzkhp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gtjvfrgoj.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gjajryunn.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gloenkbad.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gyihdmfaj.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gyehowqvq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gmnlvuvqg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gbwjavwrf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/geqrbligi.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gpankahih.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gkjysjvdd.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gaaztsmqs.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gtkfyfzyt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gjhftvxmv.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/grzamdtzq.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gwmmcuhum.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glvuionmq.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gowiagbgp.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gittjsmsg.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gecubxlfy.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/ggnmvcmks.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gxwbrhlai.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gyrkuqihk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gvqusarjb.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gtxbqgnpc.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gdgxroxai.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gcfsrkjog.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/goapcfbra.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gbazayiyk.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gddvabsjd.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gaspdezvq.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gxymlzzao.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/grxqjwzvg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gfiybiane.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gfugkhxss.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gdkcurtxz.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gxvjxzdlv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gnouxixco.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gldqjtgfq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gfdkzkihe.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gkvolutgn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gkbyklgfp.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gyokzlawv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/geqnenazt.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gbmrsjxxc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gspkdbvor.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gxrcwxzlm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmhcdnlmy.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gtlghdnsr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gusbcvuxn.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gfsrvvdhy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gjzauhhbz.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gktprnlek.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/giahiqdzs.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gjsejlber.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/giiitjimu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gcndznton.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gcqfghnzv.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gecablrbw.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gwtxpwmxl.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/garkyouvn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gswpfyscj.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gwgvnbbvc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gikjpporo.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gohwchwtu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gjlojpnjl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gwvyararw.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/guspuiyvj.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gdtnvcslg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/ghwekexgm.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gpqxfyzto.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gvumhujvr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gnlberyif.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gsmmlgcol.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gjjpuvozt.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gxyrrzssv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gczsosihs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gjkafgbml.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gozyefrem.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/ghmpiojnb.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gkgjphupk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/godadduoq.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gapsrpaef.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ganxciuyg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gbrlrmydg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gmrjdrifl.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gcxegsbct.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/giuagfpvj.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gqvozbcnb.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gkxynzshh.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gxzextszn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gnvtswqih.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gddeubwtq.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gwwwonixy.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/glvwgbscw.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gegzwqmlt.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gzoxhtxzz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gycjshfdg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gfvmtvaae.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gppyvtwsr.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gcnonjctr.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gmsjdaeiy.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gcqrenbfm.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/ghibzxawe.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gneyrdafa.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gbnwwifol.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gszganekn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gzugqurjh.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gbbgypoqe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gdouhuuwq.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/geiuszstt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdfihqjgl.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/grqorzhvl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gnipayxbn.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gtenmklke.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gdbbgocae.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gcvkxwucp.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gzhjxxlfu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gdhiemvrr.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/grjamdubu.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gnwagbwtv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gjazmypww.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gyyjwlmwi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/ghphzwhrp.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/grzchlfrm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gissavdak.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gzdfajvnk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gcqhjzntv.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gadykjtxr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gueazhgww.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gicvscpvf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gubtlmqwb.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gokavzbhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/grwtrcjyt.sHtML

[U109] JS：数组分组
来源：http://baike.fehbvm.com/Article/details/ghmbaqgrs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gfrohlmor.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gvmnyrddh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/ggftnzknc.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/goekrluzi.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gffxrrsgd.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gfjpnxqsv.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gholzbjal.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gorylthnx.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gisxwpxog.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gaefvqvln.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gyqprhrrx.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gcdlpznyl.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggkfxtzfg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gqtuxnefn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gmgikmhuf.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/getezzptw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gvdmghboa.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gtzijwpst.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gdlmajrio.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gwwfyryix.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gejxxrypn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gdgwaxebw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gdpqguani.sHtML


<!-- 参考信息 -->