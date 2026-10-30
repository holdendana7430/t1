代发 wailian999

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gaenqtmtp.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gyowczgpg.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ghmegaatx.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/glcmiowlj.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlnjbzuf.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmziklvao.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpflhsho.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmjcsny.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwyzgppkl.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gkkydojtr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvifnpksf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzszwjucc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gekaezdpn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyechmlzv.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gjolmojfu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfheghoyi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzzfgiql.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjlhwkdx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwngtunv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcbgtfre.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzodibprc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfulnqxr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnexgcaah.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjngpeevv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsycceqjz.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gomcizjgg.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgebujpc.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaitounnt.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxwljfjn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeutiwpv.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gmcaccrol.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/garyvklqm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/geofzhbtb.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gujmndiwq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwezlgizx.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzczflrh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtqakfnw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwpkyujt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrmlkkpr.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmynrvfwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxivgggjw.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpgotgzg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gacsuoqgu.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gqyvhjdrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrpwpifs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkznqesah.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzctforn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoebrabh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gqirmiuco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gywctfild.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gefweyfpy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbjikwzy.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gdfzyltcj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gqnrjzbas.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gxmyuwbbe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gqqigqfvh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/ghqroevso.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gdhimpiht.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjcvrql.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gxoiaedwy.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gruthzerw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfwatbqi.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrfomavu.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoyslxfx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnvnlqvz.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrocqbhd.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gawxwsggj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gyuyifqgg.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdtycxur.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsybfwywe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gqdvvoamr.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhubzctz.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gibelkjkd.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/glfpjieuo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrsrjnam.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gfresghcz.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/goluyufbj.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdcopbuu.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwgehcul.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgnaofm.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfetfocsd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvmatuob.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gjzphfpbc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gngtfyaxh.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gitbesxpk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqkmref.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gigujeayc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdazuvgzz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpdbsyjm.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbcybtw.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnynxneq.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gemysmasr.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvfgzwtwt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiepqsgz.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gwupzunvj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gksmquajp.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gviwbltch.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwigopao.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/glfcenozh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gapjvvgjo.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/govjpwghx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqzohyxh.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmuiouz.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqrabcwq.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgfnjtrm.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gpmtikodt.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ggpdbztlz.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/goyiszsjy.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfppdlscx.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gnelzedot.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gznuvpdit.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlowhupr.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/grifupesi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gximwhqsh.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfrjcggs.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvoxthll.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gsxyzwsep.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/grfrucgsg.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gulecpmwt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gtakgrsqp.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshqdszw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/guqwlriek.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjpiatmmb.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczvdgqzr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfzhmhth.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfosaynvy.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnqglixj.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gavwfujfv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzjgkpgj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gsedgqmtl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmsxkarc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwnvymug.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkaoluru.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/grtqqdfup.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmuplcdwt.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkcfmvutg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnwjuerm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzdnwrcsu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkzfovwj.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/giexyqnvg.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbzndjpr.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/ggbkkskqo.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gedfakhqm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwcowooz.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpleafxob.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunoluxkd.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gbkqwbdhl.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gobtwgqdi.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gzyyyxszv.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gpsuswsyx.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjmpapfeu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gbylheeiq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqwimsix.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgyhclys.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gdsgjwsfd.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/giepustft.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjyfmnovy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gaefxrcod.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtmbhbcb.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcedcledd.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/grymnfkqo.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goseejxau.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaoqrimr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gghbkxofj.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjhhwgtd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gegwxlgyj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/guigctofa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbswkksib.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhnsbvkg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gclrhjkio.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gxpfifzhl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucybzijp.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gmaddbddm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrzjdqxh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmjxzmbw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtypoumeh.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gxuvwwycp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gunvqsirx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gmnwpewbb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhueqvo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycsvhtm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gbgazrhup.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxgkdoggx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/guqslmscy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/grolzhkvn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gjcnlddpx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gcpaordey.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/godabrayn.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyauhmcm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/glnalfudr.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjhosszrl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpafkvkz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhctsppu.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsckppp.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/guvjvgjgr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gjhfwiclf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gixrgkvrn.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gadbselpg.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gusfsxmwf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gkrzdwuvm.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gsmvmzfvg.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzpcvktx.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/ggmrrsamx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gnomrituz.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gsnoilrez.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gxwyscdnf.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdovyoxei.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyvoxmyz.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoljqxok.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gkxklcive.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fanxiaobao.xyz/Article/details/gepnktooh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfidnrnxc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtihilplv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/grtbntelq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebapukp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/goepgnrgo.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycvfglz.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctrojpay.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqdrlerlw.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/ggtlhmctb.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gyengphij.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gzubcjplr.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylivbgc.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrtyului.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gnecjwvwn.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/glmujzxve.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktskgix.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/glboatiel.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gczjnkhir.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/ghjbnzrrp.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiyedadd.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgzwlwsl.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grlhfpjdh.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyfkesod.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxgrfjgpz.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqyvkofy.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gmyfjfbtm.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjlfwzqq.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gngqwnhqg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbwashif.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrfswna.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gbluzfwub.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/grbfwfxlj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikpbehnn.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/gmddvbujt.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gspjetggs.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkpnyqwzh.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/ggejwhbdg.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/guvojhrxo.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtqzjrqu.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gymlddifq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/glitdygoc.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gbktiezud.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkkyegub.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbdpajkn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmllnkzij.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gfmhpygef.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gpjpluwzc.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsbkowgbg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gusbrenms.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/givdjewbu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gurhnyacr.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmkmvrjsx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/grkswtgyl.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndcyfaqs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gitotazpq.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoiboykj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gjqnzecpd.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gextlyrkg.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcamylxh.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gskdgnagu.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmliyzdu.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gwiytiuka.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxipdwtdx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggxlzhurp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gscgyhxkk.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/glsqklhnv.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyubgmmsn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gblgszesm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbposbsfd.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gaugczqkw.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbqvqhts.sHtML

[U118] JS：开发服务器
来源：http://3g.fanxiaobao.xyz/Article/details/gaehkjuxh.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gncjtjdwu.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gzgshpwvg.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnzfsyau.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvnvzyr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjdeptni.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gletgflzs.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsvcytgt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpatsgdnf.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfjqgxun.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwimecc.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvgoioyz.sHtML

JavaScript ..... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnjjpwaa.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/glbypfjsa.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqjuiadlt.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggzwcaimz.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/ggzhieyee.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmezrpadz.sHtML


<!-- 参考信息 -->