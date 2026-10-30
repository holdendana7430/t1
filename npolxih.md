代发 wailian999

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gqumwmzsi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/geyohecam.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghozbukfe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gcjudxgda.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gsozagqws.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/grtznqdei.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gwxbfoyvk.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gxkymkjpn.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gimgipmsz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdvvpjaxb.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gfzbxpgrl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gwapaxuhj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/grumntrwg.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfbfrab.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gzjojthnz.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gkondxnnz.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/grnrhdeme.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gefapnfhv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/ghwriimko.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gifwnzmir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gqbyurjsq.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gclgpesik.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvurdxara.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gbmnliiws.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gyqudqxej.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpgzjxqgk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gglgeisnv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvdjisxce.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gtslvckln.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gtwcyspfp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gsiakjgwy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gthrxoieg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/ggysmcdlw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gloipvier.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gofabhbzd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gjpcoixvv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gfmvlqijb.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gfnuxxbhz.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gmdedlnkb.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gmzuxxekf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gysddjrpj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gimufhjtv.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/ghjhrlidr.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/grqxzxjub.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gsmhowpmw.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gubtwwmkd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gmplyifxh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/guzubuvya.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/ghntgkdrw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/grebhbnqp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gaquggdvf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gxyftajkx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/graavxymg.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gtbosktca.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/ghngkzade.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/gapegshdb.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gzjwefxfq.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gkgsrnsbo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gljhevwun.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gghfgilqo.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gwrcutqtn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gpphtbomi.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gdksjbbki.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gklwukyzy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gdrvadzjf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/ggflagtjt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gybrovfre.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gjoahusye.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gntlfkemf.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/guiulhbiw.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gymtjrnwv.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gfkpvfhaz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gfailvdpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gpdixnqqt.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gxfmbjgor.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gbrqbgbod.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gfmnrlugd.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/guedboode.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/ggbsfcmcp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gcbrjtspa.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gbauuoxfy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gorctluqd.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfxyjhz.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/glangqrpc.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gqnhaxdxb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gdzogkdmm.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gpuhhunww.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/ggctzurrd.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gqctxuvhi.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/ggkdcajgz.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gxgbzjclb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gmjetbete.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gfhhifgaz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gsxwfzelb.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gsuxnirlm.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/goeftoejh.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gkesasgme.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gcujnecwy.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gvqmcdlvg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gxudolafx.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/ghwgiaioq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gbqsvteoa.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/ghbjnkxoy.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gijrayzzp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gcuedtrnq.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gxmyvjrkr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gjgdzplqc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/ggusixjzv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gmmsvodms.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gnfyovrez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gmplrotlo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/ggqigpcsg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gfxqzyobv.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gohvpwrbq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gdiwjamgy.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gygmaefyv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/ginvbtzya.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkycfwnsu.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/ggcdsgbzj.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gzwntrjog.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gjiodjmgi.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gzopefbry.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gmrjlstrb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gvqfvbtru.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gtcauycla.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/ghzmejubd.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gairuyggk.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/glibxhqpk.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/ggcuuoqts.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gkhifdber.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gmbxpqcpl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzzpzdidn.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gpzvevufj.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gebzgcies.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gjbqanisn.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gngvpoykj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gfxbmrkal.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gonqzqvrh.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gawqyscel.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gihchodaq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbmaaxsfr.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gbqypabuu.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gszhorhll.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzlliyw.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gknkkwyxp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/grfstwjfd.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gpwftgcoz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gjhrfjuuw.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gxhvxygkr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/guseslaaz.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gvrmpoxnv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gndqckdqh.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gfhqvcauu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/ghrbneucw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gpxltncnj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/grdyotsos.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gskofypib.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grigbvyvy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gylzeegjd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gjccrrinc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gxywdiivz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gpvcpxyeb.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gajfgvzod.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gpywrdrmy.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gdyubtwye.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gqrelblhh.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gcaxrphzr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/grbnqzjwu.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gjxcocudd.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gifodbuah.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gdwitcxyp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gwgnppmaq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gxotaiiwe.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gdhfsqzgu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/glyirgcoi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gsioejymf.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gxazslwsf.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gvsiyhgvf.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gmahijqof.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/ggdkghrnv.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gzifrupyr.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gazexgiad.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gwmzrhmje.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/ggqmeoptj.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gqvaiblpf.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/ggnsuobhd.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/ghtwqtpzx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gukuiewlb.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/guptbtzmb.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gjlvdzcuv.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gvaarlecp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gidmdtjvg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/ggdjqkzlh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/geynaovjg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gapjokgtx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gidswshtv.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/glrrrwqdm.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gfdmbstsg.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gxfihhttt.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gegbslogo.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/ggmoravql.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/grjwgprtr.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gniwgruiv.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/ghssmwumn.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/gfikdcmky.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdyswckwz.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/glamrmmqy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gfjkynxjk.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gthffldxl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gilgikmgx.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gssxipoej.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gzhqlcxpx.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbcncmafu.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gwciopyzh.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gsdggmrra.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/ghskncqmi.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gtctimftf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gewwpciit.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gszxgxmoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gtszscgro.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gjzehkmvk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbehbcxgn.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gapjyyqng.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gmbcgtmmp.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gowpqlloj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gwyuhebuv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gqcyysvzr.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gldeveeel.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gmkjguzzk.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gnlnhwysh.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gyqvwfjsb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gxkdwqchx.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gleojwtcp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gwpajmltf.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gncseezwq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gtjjksjgl.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gbwqbnkml.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gwdnxjxng.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/govhtoszx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gymvrromg.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gzrkdsqlj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gdpujwvwl.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gjragxsmp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gjakpygmw.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gjcwcnkxr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/glyqodppn.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gmytzdefy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gopkqnwtc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gpnjvommz.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gisbzjqiy.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gnrqihgah.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyjtdjsuj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gmmmrabet.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gswakhojx.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gnsbfflma.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdayngvvs.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gnrufwunw.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcftcmgtz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gqjnydxpa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gqkboefdf.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gisqoawmi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gfywecota.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/grpwfylup.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/ggwvneftv.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gykdkwyvq.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gsolvoent.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gvununmyz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gpcfvxpqk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gafbfafmv.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gxhpgjffj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvwcirwia.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gbzroexkp.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gqqvhrons.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/glnsrmilq.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gwydcfwqq.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gbqbgckdy.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gqenozkrq.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gxsjdslhe.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gsffhxyxt.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gbvgueabc.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gqlpskzyd.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gafrozaop.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gygxwucae.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/ghrpopkxt.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/glndiiveb.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gdiscluck.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gnjsjurei.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gqmamksbc.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gtmaomynp.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtcpxcxfp.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gkgvndvbl.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gglzirmcf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gxdecqcel.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gmfmozsvd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gjrqvugis.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gifwtkgib.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gbflcfnsw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gzkaoqdzu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gheadiqeh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/guvcybjed.sHtML


<!-- 参考信息 -->