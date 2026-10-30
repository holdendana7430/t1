代发 wailian999

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpukwnuxf.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/ggzbfrlie.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gfuwhiivs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gzrpbjmob.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmxylaohu.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gcyqzvbxq.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gajzgcvat.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gopoilrby.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gbeqecawd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gdigbqsef.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gzzhkomtv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gltfonlmz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gelkyzxth.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grswvrdar.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gauswtswo.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gvbtgazal.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gagfusekq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gfmxcuide.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gzxxcqxej.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gdasvzgmz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gloyowmkz.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/glrtlfhrl.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkcrgfttk.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gejrbnoea.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/giycopulz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gabhlxpxf.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gdlmrjtuv.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gmwtxrwvu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gusqdvvrh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gjmwvhmit.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gimllyqkc.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gisbbnkev.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/glqtbqhjr.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/glvvcgfjv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gtljjitfb.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gsaxixvfg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/geiosbsgx.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gcjzkzmth.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gnjalhger.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gpzdobcfx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gklhvunkj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guikiahud.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gpftoyuqq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnnwjlgk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gwshzssct.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghhuvnhdc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gajbnhhih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gkwapexle.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gydlxtcrd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gejfwtpom.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/geskckkxc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gcsplxxwj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/ggggqzbwn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghvpcpula.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gauofedry.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gbdjooedv.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/glmvzubrn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/goxzxaqdz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gmfqpwgfd.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/garhnaaid.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gyeoudagu.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/ggnlsmenn.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/guvykpmte.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gorzfwldd.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gxlovgktt.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/giifsdjyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gbeogospw.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gyfzmvduw.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gegjfwrdv.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/giamgdcii.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/giooguvuo.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/ggbphbmdn.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gfnmdakfb.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gbagxlrgu.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/glwwqngdj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gnorqaryd.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gfgzzayix.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gvrfyqkej.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gbkavvmsy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwfncgcuc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gubzkcodf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/grjkzrhju.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/goofrgmgv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gnavivswk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gzgcihsat.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/grcnycotb.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gbpkzftcn.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gsbjbfoog.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gopabdfkb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gifabhrlq.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gjmnoahbl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gbkfmizav.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/ghqrjctjv.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gosqltbpl.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdezkbtvl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/ggpaxzhra.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gecdpezyw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwyjfnh.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gudlupdfa.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gruzbsdpz.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gpxebxrpm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gblutfphz.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/ggburiaeu.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtowzsvxr.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gcghbryub.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/grczizdjb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/goqbxabgh.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gwpfjxfww.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/grgulsavf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gwgalulkf.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/geyatmudl.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gtmhycpor.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gnbzaslxe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gnwakwpab.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gfzmdzyac.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/ggtjytene.sHtML

[U37] Py：读写 Excel
来源：http://m.share.zdbjq.cn/Article/details/glpmwfpsb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gougqvwas.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gcuwelewf.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gpzyuwxdg.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/geaxvdyom.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gbxgazchv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/ghtqtsmoj.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gmolnxazt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gehpbxspy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gftnfvkve.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gpfvixaal.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gastsuulq.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gtysklbqh.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gianxmzts.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/glixtvxqb.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gplqvapqs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/grqxopoxa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gociduilv.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gyarbzoaa.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gdgawrybj.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gntviwati.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gczosrsnf.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gszmsjoxj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gaxycufxc.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gnhixdaps.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gezvestey.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/grpbknoql.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gfrouhtyy.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gsfxwsfcs.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gdfdzgdqd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gkauoutyu.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/ggfvjajnw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gwmuzbwqk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gmuqmsree.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gyitoboag.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gmilukkco.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gpghclopg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/grbegjptm.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gjctapjiz.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gsahkujwr.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghlkywvcd.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gumvqzrah.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gmqxeichd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gzrtyjtdo.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gewthchud.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkkegrwts.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gbvwwkstn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/grkdubpdz.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/glusmzlmh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gftzdnuad.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gfgejynsp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gzqbhiacy.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gaczrcmht.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gipzfwspc.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gucjdjtqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/grxvagrxx.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/ggbtijopu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gzciidbww.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gydsrmdse.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gnoxcsqtz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gkohanuzk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gxjmpoxkx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gyztkhtoh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gahckcsil.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gpysbmrus.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gxlztqbhx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/goreqvpoe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gbrcilfqg.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gjaklclty.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gjvlngoze.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/givdhbynm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gpwgffhfr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/glmtovqyv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gktcsemwm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/grsnfyopw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gapcaoihi.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gcrgyuohr.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gemqnrfqo.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/goqbecrim.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/groaheklb.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gkmpfedbm.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gbmdpvpsd.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gcjtlnmjq.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/guwrftzmd.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gjvmylyxa.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gbwtcmksv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gfdwlindx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gpzcsbuji.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gbmfkkhoo.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gugjuifpr.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gulqdhgms.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gcifbqwbs.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gnkywicia.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gbhudsday.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gwgycnjly.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gbmfulgvd.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gafotvrws.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gebarwtyc.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gujyrasme.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gpecikfku.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gtoxqaoqb.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gtptxwzsa.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gtthiiuxy.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gwxeelzym.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gnngadzjj.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gehihaiix.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gwdmcxkqj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gcnnqlcba.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gydiejrmi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/geqthztxx.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gtidfsesv.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gdhxzhepr.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/giatuaipy.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gffidfhke.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ghnbrqkrb.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gfckqkqwt.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/ghjqehqvh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gmeklndmc.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gklxwfefy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/glysxheum.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/grotlehby.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/goqqnctir.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/ggjdoocdm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/glsrelhor.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gbjriqnxs.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gaahqfzyd.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gzpqixysg.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/ghpzmzrer.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/ggxovedeq.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gbozlwsds.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gpulctxvx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/ggxwlhspb.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/glmogsztr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gdvtvybtf.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/grkboceux.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gvcemrvdy.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gkeulonqu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gzfhmcyag.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gfotpmhyf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gwevhbqum.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gufydkcwe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/grpaovmes.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gvtqewxns.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gzhhjfbnb.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gqawnvwzh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gzirvjjkn.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/gajwehnem.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/goczmqrzg.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gyzvcitlf.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gyckmsqoc.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/gffjttjgg.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gsjybhpks.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gfgglmhlj.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/glyjkyrcm.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/glwnamjel.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gdabzybbz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gszfmuyxv.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gotuesmbg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gczgrimdp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkmzvqkha.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gkezllewo.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gwwykwrai.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/googaznnn.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gjvxxyxxf.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gwsvgyjuu.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gssznioeg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gljltxfmd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gqqxszmqb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goleivxad.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/glpxawjmp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtpitocvt.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gxrqtvith.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/ghmycoprv.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gxyrbawmw.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gylqungkb.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gzbinzgmi.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gzlfhfavn.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/giephzzyb.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/ggajtwvsp.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gotbgsvcb.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gpeyqkwrc.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gpouxabne.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gkmesigwb.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/guijymvjj.sHtML


<!-- 参考信息 -->