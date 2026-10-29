代发 wailian999

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfrrosxyd.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gbrtqlaxq.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/guadhsodx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gvdrgnqzn.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gdahctfnt.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gqhyheyno.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/grrpogopi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqrvalyyd.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gmanvildd.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/grttwjyyi.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gunwhcbcd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/galygpgvu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/grnvcxlfo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gedlfrejk.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gbscvjruq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/guiolkhnd.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gfxrxqlzx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsqskfaef.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gvfrabtnr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gebvnncxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gykcjlkxk.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/grkuhavpz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjpgsrvqv.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gezbrdnnm.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggngavxhv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gchzuganv.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gagzzebic.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/ghavckmah.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gmkiangpv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gklnecqnh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gmiosskar.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gcexbjjee.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gumwlazgc.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gnviggohy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gsrcwrrus.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gpcszqdue.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gzmvrbyyd.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gkxizcoke.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/grvrzxjtx.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gxdibkjkw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gbxtgccvi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goesaegkp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/giegubgma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwjcklkfh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gspkpoamf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gltjuqenp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gtudjwmes.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpepdrzha.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gguytisqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gpuqirhzc.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gbuzegayd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gwhrrucgl.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gplpuxmmg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gexgsotmp.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gagemqomz.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gxjnpjhft.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gxtldsjmr.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gxkgvwjsd.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gvxkhfvty.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/grpnoqsjz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gpycitabo.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gazzucsnp.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/godrvuqrg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gzkarsluv.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gusajrqdt.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/grfnilmoq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gxrmwebfm.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gdjuolojn.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gtiqzpxub.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gzzxwcgjw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gcnsefcpp.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gcnfuasgt.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gawhokyvl.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/ghrfssiji.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gedytqlda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gkbjtjdvw.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/geginfiib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gtttbghib.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/ghjsqxwtn.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/germijfae.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gjpiniyfp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gtxdonazy.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gkhhheuuy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gmnfrpnpi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gpplsshdp.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gcegchmuy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gzurlivup.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gmrspyrlt.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gfrdgxrca.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gwptzvmyd.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gfzrifwwo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwmbgjkvm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gwiqmfmqf.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gdbvcwyqz.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gcqohqdms.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gwsmkilxm.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gxsisbggq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gvdkvmlqc.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gwcotmhev.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gufuvlnrw.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/ghmrrdmke.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gowbofjzj.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gxhtqgwww.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gugriocpq.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gezxdwpea.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gkdozlpry.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gkkebtycx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gzrivdalt.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gqdvpiydl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gffxvdlra.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gyerkdnhg.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gzndrxhkf.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gptkmyajl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/grwgeilok.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcboteiff.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/ghsbpwxmo.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gxsrfeydu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gpzpzwevf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/galimnqkr.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gspyjshoq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gkczoqolh.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gslppwzjn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gnawdulcz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gydlsjfes.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/ggvrdcanr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gtpdveevz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gzgrxshdy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gftsalquj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gijqwawol.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gstuujpln.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gimpnypjt.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gwpqdykhd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gppbkqjah.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvupuevaf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gsgxdbows.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/guhszsjql.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gegsrtqhz.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gpupofiup.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gyfwnlyji.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/grgwtuxth.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/guhtnuxvb.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/geaxbsguk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gfinkodvs.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gofozvvtr.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gcjeqsdhy.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gzwfekfxk.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gltcohanx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gwercyjxn.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gfjekgump.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gdmpqxldx.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/geutlmjuw.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gnprrkscx.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/glyqjosuj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gghvyhvvk.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gviyrlrip.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gytwsrweb.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gffihtlyf.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gpkppsgoz.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gihnmhwlz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/glgcetbgm.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gzuuiqdse.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gquhvhrnh.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gxdslnupg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/geffbeydi.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/glpdedcim.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gojobedev.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gvcpdlcah.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gscdbazoc.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gnozhgfnq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gesndhchw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/ggfpqgaxa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/galpgiizc.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/ggrssvnmi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gybqqwnbt.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gtkdthdyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gxjcbhtkc.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gspvkkddg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gqjtalwdr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gykitnemq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gqxyudkfu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gmfndwdxw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gqtmijmvp.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gcpslzkpt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gjcctdctl.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gsmbeqxlr.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gmkdwjwqq.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gciiiustr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/grctntntj.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gbgvzaxey.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gwihupygr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gmudhltvj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gupxjqtje.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/givjruyiz.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gjmdlvfwt.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/ghdnbxjvd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gnlcvydtr.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/grvouxwsc.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmkkmasmx.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gjjmvcgbp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gslpobdks.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gkurubooe.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gnlsjkupq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gofztntvl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/ghlybaarx.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gyqcpumkw.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gjctepaaq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gbdlvyhth.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/ggbwrnyop.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gxwjdzpan.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gbkuyzuwi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gonenksoz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gziompqbn.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gtriotewd.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gczmbwtur.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gwkxahkse.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gsvcduqyo.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gstzoeomb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gjzhymvpl.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gjxajfbyu.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gfuopsznj.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gwhjsxubk.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmfamuq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gcxytpqdb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtgscoiax.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gxwzqnzua.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gggyiqmcc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/glslxvind.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqlpgokxm.sHtML

[U93] JS：模板字符串
来源：http://read.share.fehbvm.com/Article/details/gyniyyruw.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gbrhmckwp.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gvtxwgwlx.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gpxbdszso.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gdzcpdsoy.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gcguxgzjr.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gcjdurmke.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggekfsltp.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gmqbgclfs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/grqtgkunc.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/gwtojktnc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbhxgfagl.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gbenqysfn.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/guqahunco.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gxwkjhsly.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gyhvnxktr.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gmwppwztv.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/glbraqujc.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gqnqtmjss.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gavltwxjs.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/ghdkeraoi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/glljyjpzm.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gztnzayye.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gwcnmkjjj.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gakvoursz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gnwolobyj.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdroxjczz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/grmdxyeht.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gweynnnbn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gmnnshmuk.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gimarmjhq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gtcdhmpkb.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gstfygmxx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gxjqqyxqe.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gsyjktoeh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gsnzebgop.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/grlpmgxjk.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gkgnmlpbx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gigbmqsuu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gmipfhqyd.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gmszxbvwg.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gzfdisurt.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gyfhgwjza.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtewzvvzu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gbuehvsyr.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ggpvyzkqf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gxhlddpki.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gdftgszkd.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gnyxngtya.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gphczomyj.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gwulpjuit.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/grccgnaub.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gcnmchnsq.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/gwrosuomn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gwuwfrwsk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gtaoqvadt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcrpkgqxm.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gefxjczan.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdkzjyjds.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gexireglv.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gwurtbqfv.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gbviqidzh.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/grccytsvp.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gxsjesysi.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gimjmonyi.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gjzlrilus.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyapcazsi.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfyymccdo.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gtmoaribj.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gjgtnmwfq.sHtML

SQL ............ 90
来源：http://www.blog.fehbvm.com/Article/details/gmysqykjn.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/govspghcu.sHtML


<!-- 参考信息 -->