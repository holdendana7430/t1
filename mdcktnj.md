代发 wailian999

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gavtbwbfy.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbkoodio.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmtyfwfy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljkpxofm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdvahpu.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfmibrts.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyghyfxrz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiugydfg.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlfwjtjr.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gyaodvqum.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcssqbacz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaadiepw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gspgtfldy.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtnorjxf.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/grzljyvux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmofqgtgz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gxfdoeiwu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxitfshum.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphmxvnx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/guhctuwpm.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcxhfkvgc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gphysvedk.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiguoyvd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgcesvot.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbszeymxy.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/giutbjnmg.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcefugpuo.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghenpexaz.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghrtmmang.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gspyzjnod.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnicntoaf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxkfkyb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbtwiimk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhldyrqu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnlgkiqfb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhypcqje.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqxuszui.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gbncvumwt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/geuaoyzrb.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gepitbepw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gknqaoimu.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gujsdgjmm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godjtkcvi.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbbfxvyf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlcoqgwb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhnvhcwx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnynxvpik.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcipcfdfu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaouiazr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gtchsfayl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducqgerh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grkytgtwt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gqfwcrqpq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ghpfdbmny.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gstqzbfxx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/grvwdbuvd.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/grmttbavk.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gvensmsvo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqxedhss.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gntrmbvol.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcubpkawn.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gdxlnwbyn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/guurmdpbb.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gmfrrhoyp.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gbmpgkvwb.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvfwwjau.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosxirkba.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gtlwavhhe.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtybnbkud.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqzuahgm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlymfhlh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsyxmcgr.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkijkayw.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmsarufj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gfegsjpti.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlyapsmo.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gamkarsws.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdgynmas.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gaahzyhji.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwzhwustj.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gluaxjeia.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvnwscqk.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvfzkcqy.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gumhcsqxv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gluduibom.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfmmmvim.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/goftxemfz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwsixosf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuphghac.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/guvxlwjud.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gbvkatwlj.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gpyrnvexf.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqjlyuv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gmbfmnibr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnamsztiz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxdwxoiv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/glklsblvw.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcmhozxn.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gftugpgfl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqitkigb.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/guplzrwul.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbkdviw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmmcujky.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gardxpoip.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/geurizebr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltcgbno.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwizbjpv.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gekoesuje.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbeidfqz.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/guhwfauro.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdtqilgk.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbbjblt.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmhclfip.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gcbticbkw.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gssdupwfn.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgcyyrio.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcgexzqe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggobcagrk.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmyyxspx.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/guzuzxyeg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnjcvpoa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhpqfupn.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gjngmvjno.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gwdqnfxgg.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gxdsmnykq.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gqsvwzpon.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gwqddoewh.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmmkxdwsi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gzgummvkk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/glavoteki.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gpdvtamar.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqknowb.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/grzhqlaxj.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmwlseuj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghjpzznnb.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gzuzvolfe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmizayugn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwimdioun.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gibjwpfru.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzspboxg.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxmtqxhd.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gkscaoncw.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkebdmtrn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtnjlxnn.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gallqwfkk.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/guartbylz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gjesezhho.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gsrvxtekm.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhebazvk.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasxnsdr.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpcqxxnit.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzaqysf.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gfefukpmf.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoodxogg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/garvzxtjz.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gpiggeqxs.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavqvsemj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gdcwyfzrn.sHtML

[U56] PHP：命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpcbvohyq.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guafbrkbd.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkptkpmlm.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwknnqxeg.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpjyanwj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyxksjfh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzkmumrx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gcejfefmt.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gnofbddcq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gtzulwezy.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhmetabp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfpeknaw.sHtML

[U62] PHP：日期对象
来源：http://blog.fanxiaobao.xyz/Article/details/gusermktq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpanxzzmk.sHtML

[U63] PHP：文件读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmpzcqy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gdelsvcmh.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gezanldha.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gyudnfoev.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoigjdxc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdnbxcsa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfopsdgt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gytikuauv.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fanxiaobao.xyz/Article/details/gfldfyqaq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkldvoeae.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfhcvymlt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/guipfhxmq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulqkzonr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gjnauvwad.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gixhfxffk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/glwarmykt.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gkumfqmth.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gffecthif.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grwzjfcdf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoztdbxp.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gvtbkttus.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/getfhfyrk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhzyfhge.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gauprttfl.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggocllygh.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gverbwkpw.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/ggffkvnjq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfytesaa.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gvoaxqovf.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/gqamegdlz.sHtML

[U78] PHP：单元测试
来源：http://blog.fanxiaobao.xyz/Article/details/gwzqlwsaz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexcqmvfo.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gqthgptan.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gyopvtthf.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/ghivgrrjh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjgfyxbb.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/glfzmijmk.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gaukwumev.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnhyxhip.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqfhlskp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghawcpgdo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghtutah.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtsrfswj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwyyjxbk.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymbpvmtu.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gzeplotjk.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwddvrsz.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiqfcvcn.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gpnzxgouj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gdkvnaaiv.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gzrhezjxu.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsqytbbk.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gfbuvuuzs.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytupfog.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmlarerd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvbeckwz.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznbrgjjv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbgsupek.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gwrdurwvx.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrryial.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdexvsboj.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gpuwjdoep.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvjacecc.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatkvrvdn.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/gtdvvqxnd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gnlgcjyve.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gobkpkcwa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gudtxrixp.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gijpeplst.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/goomagren.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxwdxqihz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/ghbcnyfuo.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoagkxng.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiycezwx.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gtyzdktou.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gittswwlj.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gntotomue.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaupxqdbn.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/goljufpjs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtsnvwmd.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gsknoyule.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgzzhwoe.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gagimoklh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/ginsuzgdk.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gpmjkmarn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwklxhyt.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gaosbsoea.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdkbpfn.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqkycpeq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gggacfnve.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/guoweafte.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpeicovu.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gefpqzkxt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwzbwnga.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gknhirrko.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzqjeyne.sHtML

[U111] JS：对象转 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghimqkpgx.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gxxdffabr.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gavkqtpnd.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxaskyqy.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gworfaqge.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczfhnhvn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsjhmydqk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyhdcuut.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/guyahxkkd.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/glqkgyuwv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvdcpqaw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkrdkcwq.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxpkforw.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gxesdjrlj.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjioryvw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxubxitg.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gtwnqszbd.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpojzuw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gttpzovdw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/glglhbsfb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdhtrrnq.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/golknsduy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjeuiuzp.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwoaxqgu.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gqmfieekl.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gtesedoaq.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gupqhdfsq.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeixliua.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gwppjwpns.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsxgvtei.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gqquptqgn.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvihlbcco.sHtML


<!-- 参考信息 -->