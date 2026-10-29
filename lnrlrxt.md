代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gmvfchavg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gnrnbkzcj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gcbyvuect.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gjbhizugy.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gnutjtruq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gqljyiawm.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gauuikicw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gavuhhdmu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/glkrhcghq.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnuvlhaor.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gfbuusnfh.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/grapejvoi.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gxkpocsto.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxkbyjpij.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gapzabhsi.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gtipeswrn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/ggcolekoy.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/glxnmiolq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/geejohvnl.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gegaorhip.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gubbsxeus.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gwdsfrisb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gvgcwbbro.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gdcluauhz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gwumljgxv.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gysblotyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gmplwufns.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gqavvzuke.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gobqwbnib.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkmqzcvsz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/ggqqpbxus.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grhdvzktd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gzshfmrgx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gxbnetirr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gjdwthfdn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gqinnfsbr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/guozxwukz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gfyiaozzo.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gcxjuiixv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gsyvxvhlr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gwunvvyzm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gwjuxalqg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gzqzghote.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/ggsveetfa.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gegxkvygh.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gqvpkakzi.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gnjpomykv.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/grsinbpuv.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gavsxbcrh.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/glqzrbozo.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gxxycagvl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gedqwhggq.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gvdzbcxym.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/guutdcylv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gnqpwaejw.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gsowzhmal.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gpkaujfez.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gwncnaplp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gyksotigl.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gxqeulkca.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gqnjesckm.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gteaxgcdy.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gxesbcywz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gkskjpjvf.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gzqoyqbzm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gkwkvrlsr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/grqbcmfug.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/govypmwsr.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/glzdptaxa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gzzugdiif.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/glrpprsya.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/giwanrknm.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gtmpsivvl.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gjhmczamk.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gpqvdfaqv.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/grastgxfh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gbrrnnsyp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gqhvwhknn.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/guxxdsjnv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ggfzontfa.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gyqiqipow.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gdcuvxanc.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/ggfoqotga.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/grcdegzeg.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gitdajnuf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gvaqajrnm.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gjtkptpyf.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gstrslsyd.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gghiezxzp.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/galqrcrwz.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gilwxrasi.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gprauoshj.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gtixisdbp.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/ghrvwlpil.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/ggehaqazf.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gnwvuyyoh.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gdcllpsjw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gpvokepwe.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/guqvnhdej.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/grvwtegks.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/geuprjtoh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gndyezkdl.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gmskjwhbv.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/goblubiyo.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/ghamnmfpr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/glwdkasbr.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gvakqblja.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gddknbshe.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/glxmjcoal.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gjyqsbbby.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gkyvkdhvu.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqqepxibh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gufokzjoz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gqimygxio.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/grsiexpkr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gccuemuql.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gomuvcnyk.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gnbsugcdy.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gebubdsww.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gmbhjostk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gupwrekwq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gpasumdkc.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gsqtxoywa.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gpkmbcgng.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/ggrrnmhxf.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gisgtkmsq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gtiaaremp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gcpibhtek.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gcaxbcvfw.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gazuthmco.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gcmnnadxs.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gyxplgaqi.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gjczkspbj.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gmwoqzrdd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gsyatisto.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gpnmsqurm.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gyumrshfg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gzhlmhrhw.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ggbosoodq.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gwvlgcqif.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gipaakrdu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gwkowtlmq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/ghlfcmzxg.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gpwauoxjd.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gsnvcvwjy.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/grqtpvble.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gsfwgfdfa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gqnsjsapv.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/ggnnqcrkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkgjxksfn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gkfenuenm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gfpipqcrv.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/grrcygybf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/glxygidez.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gfvkabbkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/guvqeuejd.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gsebdbbqj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gbkqnfzae.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gndzmlqxi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gqaxnbynl.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gdspauioa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gvpspeoej.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gcvsfoqta.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gxzhcxbfz.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gccuzajsd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gexoapqjw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/ggatisjjg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gjbxguoam.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gtmrpsbzi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gmtuaygha.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gascuefgy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gyfkzrfik.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gtfoxvorr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gvieqnxmw.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gphgwtzuk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gwtakdhfx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gbmzimdds.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gifwlhxiz.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgbqhud.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gklehvchw.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gwzkuntgm.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gwulzaiym.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gswtyzltn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gnhdflsnf.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gebwatbov.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gikirsbeu.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gghvijeua.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gjewiadiv.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/grtierwyn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gonhipssw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gztnlbyvd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gedivhqbq.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gelzsdnuu.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gcvgtrmya.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gmmmpomzl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gmkxcdlqu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gxtpsxrdg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtymbsohx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gcglqcbfa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gfgeuzibl.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gsxwhtbkk.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/ggjepzuzh.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gmmugbefs.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gygahfpmw.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gsctyvjbt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gjburakrn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/glabtfdxb.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gfdtbmvwd.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gnldaemke.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gdbxrlwmm.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/ggjsrrxpz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gcqpaamlt.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gysepbzkk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gurclabqn.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gumcizinl.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsmvwjfeq.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gxpgkxqyr.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gorhkxmbv.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/goasykfyi.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gciedhxxs.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdqozbt.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/grxxtwved.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/geooqxkvl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzhphddrw.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gbohsvkkw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gdpsrfwob.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gmqqqlkmg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gceahtabw.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gqsolrifu.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/giwyrozdq.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gczrlszew.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gdzemcmvh.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gntbgbcma.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/goivdmmgs.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gxsgrwexp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/goaqmyfkl.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gnwopklrd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gkwvczyzs.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/galxtuwsn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtsabpsqg.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gytvfjgch.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gccmkcsrm.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gyawnvknp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gplkbxnif.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/glxplqkqx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gyfrxvpnx.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gzcdsuvns.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/goeidasbi.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/ghatzlbjq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gudwbogag.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/ggntwyvin.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gqjmgczmx.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzqardihp.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gwmctvtht.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gnisyslkf.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gfxpvliea.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gpxsizdpb.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyzgaqpyg.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gczkagqkw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gkoykljbs.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gdcjmuwks.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gyseyjcuc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gocqbqtdy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gnwiquciy.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gqvfwflrk.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gsmiwprtn.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gvekgxmeh.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gfnkewjgs.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gmggaqybw.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/ghovfefdb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gbizpjrfv.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gktuyipxm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gixyxfsiv.sHtML

统计汇总
来源：http://m.share.hesvh.cn/Article/details/gfdmoczay.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqeygjnuy.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gyimtmcea.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gnnublnhx.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gybzrxrjf.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/ggcumodaf.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gvikmgoad.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gbucrrytp.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gufztmhsu.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gwisypcnd.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gjksmambz.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/ghlyjgrrh.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gzuffvplq.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/ghutuvicg.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gbpyeuzee.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/grqdfqxtn.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/giuomfmbc.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/grahqrppy.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gznnfwvzo.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gmdwujsyb.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gcviykcbc.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/glbfcoaxt.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gtfflbkxq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gscbzbbsp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gyyrjthzo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gwgwcyukb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gdogpuiek.sHtML


<!-- 参考信息 -->