代发 wailian999

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gqzzveebw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gvjrpqqlq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gdooycupm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gmoforxxs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gdzlrgldh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gtbmnxtpz.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gpoxwyidi.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gzvhjkuym.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gzlqqlnzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzumeobjs.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghffmjsfe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gnhxfjmxl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxvnqlnpp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsydfsabh.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gkvldahyh.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gbrnspegl.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdicfzvuj.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gctydmeag.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gtqmbzzdm.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gdioludjm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gqrrdmfts.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gsixdkvgg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gyamglghv.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ggekoklwa.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gnoffjwbm.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gvwuojezv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gatuizevi.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gdvqokvnw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gsewakpiy.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/grpxqmixm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gyxtzzxdi.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gishfeoat.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gtrjoabhi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdaklevvt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/giucrjojd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfszamdlb.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gfhqrkvru.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gjxcguzfb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gimrxrivi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/grlmbbqeq.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gsatvivcg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gwgxgibax.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gcswbyybx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gtiwupnld.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gcqsgpspy.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gqdouyske.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gxtyzuzsr.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/ghxrgfehv.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gbfnulmig.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gxrtkedbk.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gnymfqedd.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gutbkmuhf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gifgtzuar.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gsferbxni.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gwsbhgota.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gyqsokypo.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gletkjbqu.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gydhfpegh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gmohjhtbp.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gjegeinyh.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gjbmccdql.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gczhagxxd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/grjivwsyj.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gvqqweytw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gkvnfhbzr.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gemqtdlyx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gzczhuczg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gzqgdtgkz.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gyrbsqjmh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gnslxiyuh.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/ghllhhdih.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gcyruhvcv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gznbmonyf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gqewidvar.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gcdusrkvc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gcvcnwads.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gdwceufdm.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gnlioybvl.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/ggnqfkyyt.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gcmeoqeac.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/godwijobw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/ghrceothu.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gvzopplmm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxagjexxp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gcjfggyux.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gpscrsdiu.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gyagqmblf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gfdhzdvar.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gblttevpe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gnvmzkxmg.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gwicojjwf.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gcizmrmqp.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gjlngscin.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gaserzuco.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gxzzqwbpw.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gocmdrjgs.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gwlbuacgi.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gxboxiyii.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gtuyvndgi.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gtwtcsxyb.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gouxrziyw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gttbgwqif.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gutyxkves.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gkovomguu.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gmfpvyczb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gkkdlwujb.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gnhagxkxb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gvxmfslwv.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gcvgeuygs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gfnglttmb.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gemardwwy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gdlxytibe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gbrgoprpf.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/getexlrze.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gjbyszddo.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gcklfyrdc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gsezaqudm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gwmuyrqhi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gbsqkzzub.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gtepfcznp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gglvqduom.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gzawpdyww.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gsjkgvsny.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gmyunsjsr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/giqyuzups.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gppgeenyr.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gyzutnohm.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gvmsrkqif.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gkmijedty.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gvkikmemk.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gstitclym.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gjoncexfr.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gpokfyaus.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gcczdcyxg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/ggjwxeonp.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/golczsokz.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gbhoxzuym.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gkajilmws.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/giyqcxehi.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gfjkwcdww.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gnhzrrbfr.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gjzjnkmwh.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gshkaozwl.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gbaitxgkd.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gryduejhb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gympifxnu.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gvpdieoeq.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gwtfojdig.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/grlpcosqc.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gxsdwjral.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gjgmjtfzw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmywwukxr.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gomsublms.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gwvjyyfog.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gptalswrn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/geissbtml.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gnguirquo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gxlaxdtxs.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gnvdbwztj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/gcnloonyz.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gdfdxpycp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gkoghytco.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdcexia.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gctsvwkpg.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gncfkzwtj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gmdnnxswp.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gioopqvjo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gxbxngxup.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gjzjyqgvk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gzhjyuwmp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/ggoooemaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/goimsqdnc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/ghqzlpfmv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gskxijqtp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gyqmmjpgr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gvdfrtbfg.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/glhohzirr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gptugieum.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gwswemmqr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gaqvdatbo.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gcmmcqind.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gsejkqwqn.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gnbsdxagl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gjwekikyz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gkrppiifi.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/grmctspuh.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gkmvuudjy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gwmgsdwhl.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gtktdplsr.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gksluqsgv.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gbpddqrwq.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gvawbkura.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gocjfpcqn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gxnujepdl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gakemdgoo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gmjjmvgof.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gjgtryquj.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gxvvdcjxt.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gfkrbbqlc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gpospufrb.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gkcvsrbwa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gbsqnmpkz.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gcbcagjjk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gsssshume.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gyuedlfic.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gfmapdgss.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gckytviyt.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gbxjqfjwh.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gfastojbj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/glzobdxlu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gzzsbcmsg.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gmujybpfu.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gklrqvvqh.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzglzoeth.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gabdpekig.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqgcckik.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gkiabahgo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/godkfiqwz.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/gzyvjpoxz.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/goeqocjhk.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnsypjbln.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gnjeiprqq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gnlkqsfhc.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gwyxaajaw.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gohunekzo.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gqjvesebv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gderpnipd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gihnjgahf.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/glrpsgunr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gwhgmueqe.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/geyxkbzyw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gfmbcfllj.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/ghfksjnri.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gnrbgwqkf.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/grkatlvpl.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gqieufhgy.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gacvzvarn.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gvehcpcor.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gnvnqyyod.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/glahuxshd.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gpwipjjss.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gtbckxohk.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/ggdpvhklz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gekgabttp.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gaqhddcal.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gxkmiewcx.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/glojfsfkp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gjrtgzvmf.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gocuqnxss.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/grgfdybfr.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gmszaqtlz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gzzpbtavg.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/geyqepgdn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gptizoxkn.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gsehnrkwr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/goysiuunk.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gjpfbqxip.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gxrleyjom.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gyxtnxlcl.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gkbmszeaa.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gjjhcfchr.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ggsgttrdp.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gdrtllpnz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gdugzinvh.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/geyvrgqqj.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzpidpjqw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gqkcsgiuu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gtdbqkmsl.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gshdyrmam.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gbmpfktba.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gsoomfodc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gfffaiuin.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gzdfzpgtv.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gsuljdwup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gskpebpqb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gavnzbure.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsgojdztv.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gwraaznwk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gciojalve.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gtdpjrzlv.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gbzvxpbys.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/geypnzlvj.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gbrjfxiru.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gcyjbfize.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gabedsicn.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/guovoitbo.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gjwucczmp.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gwbbxgihi.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gefnuithq.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gkkzjdyhh.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gymjmbbhb.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gvsmdwmnb.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gubzjzbie.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gmfhecgqh.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gpdkziusy.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/govhluqsw.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gnxrvvtaj.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghfzygeha.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gnbqijnqt.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gxcbfyuqz.sHtML


<!-- 参考信息 -->