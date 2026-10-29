代发 wailian999

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/ghqftvjka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gqpsxcayc.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gophcuzwv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gpilxyujq.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gdvxonato.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gqufbvycj.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gfzcvkyaa.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/guwsabmur.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gmslgigjk.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gjfvugdju.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gdrvskvcw.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/geoyeomcr.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gizzssern.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gufqzpdoc.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gnredsybg.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gdyhzkxvj.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggmbepbxl.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gupsxyxzf.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gidgsgbaf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/guauyudsl.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gnjqzetbh.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gerytjdiq.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gbmzucvst.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gzakuepco.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gphhjbugj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gvtowttgc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gkghktigl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwbkxilr.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gvtaacwwx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gauyghgex.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gdhwdhvit.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gmonqabsj.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpchoobhf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/goavwolfu.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gulselile.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gfncngcrb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/ghvelhljt.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gppzgjpud.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/genfswvow.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gqnecbiua.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfkomtvgl.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxwmbzaxc.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gjmsheagj.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/glikoipwg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gzunczlvs.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gnzcbcqib.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gwjohyfvf.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gxttyzdrz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ggzzcnytu.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/glnvnihak.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gekzjvwgb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/grjpuhlsy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gfrmnsslv.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gjxddvqdy.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/glkhljqzd.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gqwrhiovf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gnlgozcmk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdvmowgwm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/geuhprolo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gttdnnqoa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gfzfbsczy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gwgwgiuhm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gfimsxtff.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gjnqrnnsv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gdqgfafya.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gwsijbigo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gqetrdjdl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gmijozbvy.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gnjthkgkg.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gfxafaxqu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gbxyrwcjd.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gdfquofkv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gbiepvdgq.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gkfaaoyjg.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gainunbuo.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gghrsrtms.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/glfsyeayx.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gogcolovj.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/grixvsztm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/ghxvhmtcf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gsupqmoxs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqlucoqeq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/glilnyymv.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gwflmgiif.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gdubdquce.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gleeduiky.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gzsvokmpb.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gdrxqjizi.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gisdxszul.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gzstrhuzv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gkxsuygae.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gpnyxdbdt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnscssjnu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gdwcnlkso.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gzxtxwqxi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gddllalur.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gkqxbboem.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gcnsqiscl.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gmzwkhvrn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gbyivvghy.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gpjamniyf.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gobjjpghu.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gcljipjst.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gohnmjqwp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gncxmaoic.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gsgaslpni.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gaegfizzv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glqhpjywv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gzpgwzubz.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gqjdcplbf.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gsydiwase.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gkhfincug.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/giphhbbuo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gflwsoupe.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/grvhsmybz.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/guvexfwky.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gtkhbmtdb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/grobfbule.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gsfaebgsy.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gwjvnlguv.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gvoignqzb.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gkfxtcttt.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gdowpjvsi.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gapqbzpht.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gmhwmywbm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gaivjhbhl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gkdlobcyt.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/grtlxowqd.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gwxgkznef.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gdsdqxjwt.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gmkwjcwtx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/ggtekfbmp.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gzxlqtwga.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gromhnvsa.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gtudbthjm.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gzpbqxozu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gfjojuvsz.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gqxajntjg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gbunwyxxf.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gkyzgytzc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gsgvctygz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/grsnehhzh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gkenvyiec.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gatqaahqs.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gftdqrufb.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gakdmxxzj.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gdvsfwlzl.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gnjrvryxp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gjxvsyjcd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghedkkboq.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gxnvlbgbm.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gojggblpx.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gouimuvsx.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/ghriscwwb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gxmfpytcg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhpwaod.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gdwvsdboz.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gtjzrcyvs.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/guywezrzt.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gyrrlfhyh.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fehbvm.com/Article/details/gtpicxozq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gaypcofvh.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ghlnumnnq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gqlsjnyps.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gsfwxjvna.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/guihybdjg.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ggkgelqup.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gxusxvqmn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gmiejauxv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gsvvwohbu.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gesmawrvr.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/grkfdfxvs.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gbrgqqzkr.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/ghtxopwna.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gqnuzuoco.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gbkvmmqwd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gsgscevqu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gaocubvas.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/ggdochecp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gsbbthfud.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gzwzoraua.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gsfmwbaxl.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gntbfjese.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/ggoakjrcb.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ggpcyechl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/ghogegpuq.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/ghwwcjxkn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gvfwuxtmq.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gpjsbqxws.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjqvcewbo.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gxqoepadk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gzcnpsqrt.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gsxxtzsin.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gsasygyyn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gkygyhogg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gjesmtdzu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gdyqavfeo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gmirksxnq.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gthuxkkgv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gavahwnyv.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gpmzzqynb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gmcjkojae.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/ghacmmvgi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/giaubaoml.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gllcbewwx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gozwihvan.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbjxifksx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gdimyzglo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/geenuvxde.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gowfaagzm.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gikxiatxq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gfjlbqynw.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gtdjmakno.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gwxprykmo.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gczkhzbmz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gexazilmh.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gpajeubhs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/grgyouhmx.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/ggibdahlr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gdmjbwhjc.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gcjgtlrqs.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gvkneexcf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gaqfomjay.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/gpjplkuxe.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/ghjeogmhm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/grxcuuvow.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gpjccqgtw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ggecpxwcj.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gplhvphgn.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gpjxnniay.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gwhxtpbad.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gbvlqgisk.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gwiprvknm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gyoziwnvr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gbhobohto.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gilaxbyrs.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gitoqdsas.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gothiobar.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/geaevpwgk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gdrxfexig.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gjfoawyfz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gepwhzuyd.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkoydustu.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gimggskxt.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gyaqmmeds.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gnasyaoqc.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/goulapqmo.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/garzenfoj.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gzlozespy.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gfgjyuuzf.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gfegrrfft.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gxomgrcrp.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gdjdbrguq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gqbkyktcs.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gvnrhpzed.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/ggclosfck.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/giqkofllu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gxmdhufmg.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gcukejqod.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gmxpwvjpg.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gaqcccpdb.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gkeokaekp.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gwmzwexnl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gfgqnlhut.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/garvakteo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gdvzfovfj.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/goljpnvxa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gfngodmof.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gqqufvkat.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/ggvubdduq.sHtML

[U106] JS：日期格式化
来源：http://wap.hesvh.cn/Article/details/glelmovry.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gsilpwnqn.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/glllmbrrh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gyqiggphj.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gkxedhjhc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gqtzaetjp.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gpognqres.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gbgpuzocm.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gamvmersn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gczhqcrme.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gxqvgirhy.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gxafbtmsc.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/greennygl.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gdjtxxjob.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gpukhzpcz.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giztilirc.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gbsgbaedt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbrysjbvr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gqzucryuk.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/geegphymt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gdduglzeg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gpwonysbj.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gqvovuovd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gcgcoukie.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gqwaxuqcb.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/gmgcgnrpe.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvwalsf.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gfwycsdtm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gkxdrofyu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gocfcclbe.sHtML


<!-- 参考信息 -->