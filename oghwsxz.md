代发 wailian999

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/golyanqaj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgqsotbr.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqvqfvmr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaxszxhs.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkfkohnn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggylblopc.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqusruqjv.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gftiuskif.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givhlttdl.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gisffkumx.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuwqdpgj.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/galhaaxqx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnyyalqs.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdgocgsn.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gzljkwyxo.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/glevnrdgc.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlxkfbky.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbzionev.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiysmngs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gctydctep.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gappsektu.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gvmyxiihh.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/guidizmcv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjfrcohy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gawutayxb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gefoochjf.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjehwmgp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goktnpswt.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guapulqrd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/glwtsqndr.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzbyephkn.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxpsvuuh.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvkrjzmy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoxfenut.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdqratynq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkggsawyt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtonippyn.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfpizsier.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gdnmkfssd.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyggyzdsw.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxvyvxcxs.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdfcdgmua.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiepvppo.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbfloahay.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggwcfbzn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtwaqfurx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmggcmufd.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gbdokatca.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhxivoiq.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gahbyjbej.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqizaxibv.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gumggdjyz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrhuhzx.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxeoqgyx.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyggzqyw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciqsfqkc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gapqbbtch.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpfcyipcx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/goojqykmy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjjvzgc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnndmto.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/glezzjees.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvufhnbp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gidnnplop.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvuwcxle.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbunqlde.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqweketq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdsygoyg.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gogywswua.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/ghoctalid.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyksgdcv.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gihlmnlvg.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gwkannuqt.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ghiflhvkh.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkndogfo.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/goahblryf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuzwseey.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gilqidvwk.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsblegql.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gowolhzjw.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxxfqdowv.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gayneuzpx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxvlnjra.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giazxoymp.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gfkdzysud.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfitghcbe.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfyeoae.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoialefa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlkivrkp.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjvcwgbq.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/giotqawrd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gakygcorg.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gocodnplo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/glxqdiwwo.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gywqzhxmy.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjefjikga.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gfnjluqvv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvzelnbk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/ghqpiggmn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gatgtoddc.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/grvhlundy.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfuzgqlf.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gajnhscbi.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuogmmug.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggtjolshg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gbknczuvj.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcekmree.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoqojwet.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/ghateevts.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gdcgkcikb.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gejrmjwih.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgqlguid.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzvbjvkx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhejtqtl.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/giequtqwy.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gqknwlhzk.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzeudoci.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuzzalvh.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggsvptbbz.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpckvvdt.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnneapjbl.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrfpnljj.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyrfdetwv.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gvagmnslm.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gddyodhdo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmcwvded.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/giqebobsc.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gecgsegpx.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/giohybomf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadszmrbh.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvuetuiv.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gbacniays.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gftqozjib.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gzettbckt.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidxrzam.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gfwgxlvkj.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/giapkymem.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdndyszau.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gagsroxej.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grdrkcsge.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelviijfq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoapfofk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzapdgul.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grhujhjte.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/grvcgdgop.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gocqnrvwd.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzjfkwvk.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjyrjcin.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grihfxuhz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glsiwhnzo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnzbshrb.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/guprjyoke.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdguvuoyf.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/glnbuafrn.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/goptoinit.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdywrocuc.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gftbfazoj.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzsxjswl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvobthhc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmytzvedd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilkpbrpq.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gnnqfzmql.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gejzhzeue.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gquczmelj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gtfyaqpjz.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrnojuq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjupauf.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gggdaskzu.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gcrxgybob.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/ghttddvjo.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwwygfzi.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhdopjqo.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggjgkmvxw.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggzcvyfth.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/giaecuqaz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnqvczpz.sHtML

[U59] PHP：自定义排序
来源：http://baike.fanxiaobao.xyz/Article/details/giwnqfybj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gijbysjnd.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhhpucxj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/goggibrgc.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/giymrafsw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnglexwzd.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gmtbmkpnr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/givsszvho.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gwdujwrre.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlmpauld.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grwsfmryi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gatxtbmkn.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gcofgcuxw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjjgmdqa.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/guvvgcjle.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gkbhimije.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gkpnkdkxv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/glolzerux.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/glnqpudrm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gguolvevt.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjekgqbbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gydnuqsuv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fanxiaobao.xyz/Article/details/ggjtbbqgi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/glihyfnoz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/giioyewia.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/griwyyhfm.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrvphlxb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/glohuvnaw.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgcpdikn.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gzuadstws.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmyeofru.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbegitt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqcdyigc.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxdljxql.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gomxguadb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gijeonyhc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhoftotn.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gpfixhsor.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuofewdx.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gxqfoaykp.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyscvisl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzbbsudz.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gnbwzkbph.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gothggshm.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgoxjnzr.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gbowyypkt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfpkstwk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxhbrvnt.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfeqzgyc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gwqfnzhzq.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrbycpdj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrvbqhzx.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gyrizkhep.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpzmrobt.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gaxraqugb.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gkstdvbsw.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyinvkat.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzydpeq.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqbnkgebc.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskbmkyur.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtsvrsxq.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gytutzyaf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqpvrkal.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwzkquv.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvktibod.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gxwsciufo.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ggdywtlml.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gllzguunl.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisgqdnsg.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gfqasbasz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnuxtrbo.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvglvrag.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gfmrhvmdy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfcbepbt.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gjewprhci.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghuybmcxa.sHtML

[U97] JS：并发请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmvrarp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiyjljvj.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/goprfvaxf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gfhslddht.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gjbrbgkig.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gtjcwfwuc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmxtxaib.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwraaekb.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ginikkwml.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/gtgxpszmm.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpudvoeyg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gywsypapl.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqowxxqs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gufkcpwbg.sHtML

[U104] JS：防抖
来源：http://baike.fanxiaobao.xyz/Article/details/gkilejmsf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxewgqp.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gncxqvfrn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpcspodw.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gbujsdduo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gypbymfdg.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbihwchxa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbpvliiw.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gralpjanq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzcavybs.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gicimduqq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/griacapsc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghitaeohn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbmmzdwk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsgagbqi.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gyqsukimj.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/goceheywt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxciwnqmp.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gqksdecsq.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/grjhwovxh.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grtykglru.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gcmuwdhli.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzkptxyw.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gqerqwgof.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdotrgllr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxazfwoob.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpxiofsn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gbipgcbsj.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnarlspxw.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/ghjmjzukr.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gqybfijwf.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/giubfxiuv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbbfnjz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gpebmepsv.sHtML


<!-- 参考信息 -->