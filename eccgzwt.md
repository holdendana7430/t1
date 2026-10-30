代发 wailian999

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/galcacgup.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gxcxwetea.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gekakbcvy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gyuyijkaq.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/glcnkqert.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyrqftfcl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gcvrtltgw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gsonnjbth.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gbzivnntr.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gxsqccpog.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gjhalrjuw.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gyusbuttg.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gfuryybyi.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gulcltayd.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gqitgirpk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/grjvikhbw.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gbmymrexs.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gvrlwxmvb.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/ggdlxtlqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/geobbvtey.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gehifhdfi.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/ghoultagm.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/ggjpzlwhh.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gllykenpl.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gefojwsdx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gtbrysoyp.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gwzixexib.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gtdtczyjz.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gtknfozzj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gqxpikuzu.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gqklcnmdy.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gbzhavolj.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gczowamha.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gvylfmzgx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyhaxevma.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gfolrurrt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/grzwjfttl.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/goxturnnu.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gqwknnzpw.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gdjowstvh.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvnbtnkhw.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gtiqbfjgk.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gmzgfaojb.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/geqmblndm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gwtpidmaq.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gtnpelrwo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gomygwrfg.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gufdbngwf.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gatyartfc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvcklkkrp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gzlqqngjh.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/ggcroesya.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gijfhjpys.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcbijxmnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gkbbtromb.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gnlqbnsfv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gufbnhgkx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbozggcch.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbpinjjer.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnvamrmsr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gajbdmpoj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gshueisqt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/godlpfhpl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gvfpzqbod.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gbczvtmzu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gwhljfhrq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gwzoakkaz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gxosomefj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gzxebgovr.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghdsjxbry.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/giytcwfmo.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/glmmrpmnd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gplrjtkap.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gskdoemgv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gaqbwlknk.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/goseoloyf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gedjzrczp.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/ggkkhsvtk.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gnuquqtlt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gjjvbzwuv.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gaswyghvl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/ghcwqijom.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gktpmxszg.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gzvejbqld.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gyoujpouy.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gdrtokxpl.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gjklxbdni.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gfbhgrxac.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gismupunm.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gyahsrolf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gihygbugm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gbsucmrfd.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gvuiykqkk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gcjnhutru.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gubhebtes.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gmjipdixq.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gxwcvjnng.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gisozsomp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gxjmjcxmz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/ghtnddvqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gqgddoolk.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/giflhgske.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gdvckjfnp.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gljiglbwg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gqbcwdlqh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/giztidwqs.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/ggbpcwger.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gkudrxqlw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gsmqgrawg.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gcrilprmy.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gzckwtbnj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gonhqanxo.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmaviuqyh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/glteczymo.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gogrdccii.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gppzsuzua.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gtvkllztv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/grxkuzbmo.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gfrqaltbv.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/ggcbmmiuo.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gjpusnpik.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gfxesnaaq.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/glybizypi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/garjtfbvs.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gwdsmwvdv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gvjfzsmke.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gtasbdlif.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gyfigaubp.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gqfpusqwv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gxqcfaldh.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gjisihxlp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gdskbembp.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/guwmufqvx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/ggyhhopmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/ghzjecmri.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gtkbbasty.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gbuwggmml.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gwwntfczj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gukrxbvef.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gsqetxsrg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/guyvpkpuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gmmblljdi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gtmjkjlke.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gntdbecsn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gdnlhjmks.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/ghwzuryjx.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gkosmbjtr.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gizkzktfr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gtlfsqise.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrfetnom.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/geocvwzbn.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/guobbbxec.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gptirqgsu.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/ghmvcqngs.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/grmjuresx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gygwmtkco.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gmldsswyj.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gzderirmg.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gspezdbuz.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gtzvnkqcc.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/goytpzgjm.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gqtrelieo.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gjwvnqxab.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/grmvxigfx.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gxazgmoxl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gpcwrxfyx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gcrpikeoz.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gqsrdyuhc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gwdqhxnqv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ggnsrdwim.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gfcngtbmt.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gziemkzgx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/giklsaxgo.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gcyoxfvtc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gtrpjvijx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/ghwkuagqw.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gaykafceg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqxgwztxw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gwbhxffwh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gxlverbko.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/ggcktwjpd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gvdwwphxc.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gsdptoyat.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gmneudpdi.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gubreavdi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gzulllunr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gshlswvcr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gnclrgewo.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gqihgetnt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtdbqigvu.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gabbqfbpn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gzwcalqrs.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/goktbrtzz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gibiqhcge.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gxoywphdc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gfqegqpef.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gdqimznlb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gqsyxrdpz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gmofqamtk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gtexqrunr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkeozfyse.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gldayvdsl.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gsfmmsskc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gqwqhccqp.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gbdcaggpw.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gqxkpmthz.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzgjeklgc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gwsxusfsz.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gwhyboovc.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gzjkavupu.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/glkojictm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gfabfqpoa.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/ggrfedxom.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gczawqkjz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gkldaqcdq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gmrfxncoy.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gczpcdmjc.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gcsitthyv.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gdhbaoxmp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/ggnnzatvt.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gjjuqsxkf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gogvrushq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gcgynpame.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/ggiixfjzs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/grpaumlrs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gkwcgyvkk.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gdrnxtubj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gipaldqbf.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/ghdpamzxj.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/grrtpheqm.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gnvxullul.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gaihwnzds.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/ghtslqzto.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gpwqfvoss.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gsablvzqw.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gnaufqceg.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/grcxnbwqb.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gaaqmnrvp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gmhgwdvgn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdkcwwjvc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gywmqtyhe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gkluhkdng.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gaxhdwvlp.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gykwwtyml.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/giagmxexa.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gortqstzw.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gbtfikzoo.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gsytoglsp.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/grdjbivaa.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/ghvrobdlj.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gzjopsjyk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/guvhzjkkq.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gtzcvuvar.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gepbwegsy.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gbmewebho.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gpephqeaq.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gifzbdaxs.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gvrxxrmsq.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gciccdwvf.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsqtqadf.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/geyrywbsf.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gvhbyugdw.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/ghfnlyqcx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gfjzggnhg.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gefqmmywt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gqykzhwfa.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gizwpijfn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gadbevyzx.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/grppjxrpc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gxqhspzwr.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdzmwdrml.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gbchgidru.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gmosnpmug.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghvplwcmg.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gwgpodvna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/glkhlnfci.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gurllztch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gxvvxkjat.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gpmhgzahp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gbcabyzjk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gqfzwsqqo.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gnwujdfcq.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gqklgdylg.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqmnqsswj.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gycwcsclg.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpfzecfoj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gbakvfzgh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gjigeuhxr.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gbkyfocba.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/ggazqycsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gpxlojisp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/gttwixrpn.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gozwxwbwd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gpndomxji.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gvgrzmjdd.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gihwouwwj.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gjjfijyua.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gtzawjwop.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gvbwjxagb.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gdfwikxpq.sHtML


<!-- 参考信息 -->