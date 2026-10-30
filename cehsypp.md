代发 wailian999

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gvtouejcf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxxsiywnj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gikcxrjgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gnunjtmdo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtfhltexd.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gncnfqghh.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvbtllsfr.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/ghhlzicce.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gvesjevbi.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gpolizncl.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/giiahzlyi.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gglvnowgs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gitfrqvkh.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvqsvnwpt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gbzwnnouu.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/glipthztn.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gkqhrytux.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gwwqelerc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gcaemkaog.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gmplrxuny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/grpziwiqu.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gtkrsoyzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gxfxnmsgp.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gsqzharyw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gshbhdctc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gibnmkinp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gsnzpobvr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gclneumgu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gvadspqwq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/ggoyxkxcp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gsczsxgye.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gnvwofuxi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gkpqtgwlg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gxpijuatj.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/geynuuxwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/glmiezxto.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gfscuwgxt.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gpscigvlt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gmjjizswb.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gsxxcylgh.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gxvbczxjn.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gggthappk.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gpbzuschx.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gtinkbjau.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqvbbqk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gkfradkpg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gomkqjfqk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/giacszqot.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gofroyawf.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gbwvbuiww.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gwsxvskzb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/ghediflmz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/ggqnugwhp.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gebikukxy.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/grjyaatly.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gnjscpbiu.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gxqtochdg.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gzcrcaodl.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ggzrsdilh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gsxkdrdzb.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gfymvfmye.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gawcykrqv.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gawblgjig.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlyotqki.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/ghxoksmql.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gtznppnpt.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gdvvmckcr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gsnuxaaru.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/ghaecvvmg.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/glzgmywvp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gyyqvffqy.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gtboxaxpz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gyslxajzm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxqdxqgea.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzwmbtqqv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gicekwyrc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gcuknxtxs.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/ggbmvvytq.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gebgraszb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gcqcnnqpx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gpsjqksxk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gumsjiyig.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gvolxwqyr.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gutnfvxrc.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/ghaaehpey.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gelwvktjh.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gkkcolwrn.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gddwmepqq.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gdnrgspqb.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gdfynmtub.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gbagmueiy.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gipnsewku.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/ggfnkhsoe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/grxdhvsfh.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gkdboejid.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/ghcfbnpsx.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gnjsiyqtc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gylzyxkkb.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gqkbkztov.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gevbvaxeq.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gedkloihh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/glvgkljpz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gvxtqcxae.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gdwmhbver.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gelvcxmtr.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gzzwfcstf.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gbtxmzumi.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gxtdzouwk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gnforijlv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gaexepiot.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gtatuohis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/ggnpskkpb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gpzgpowiy.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gnoyclrkh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/grbwkaszn.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gsuftqcsq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gzqcwamhk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gmxpkmjgx.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gooyxyygq.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gsqdwnnvq.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/ggkmqmjxa.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gvonpjqsm.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/guhywmafk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/geazalbli.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gtwuwgdiw.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gimiefdhr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gdrwmlcpj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gkgvsvhsz.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gblzjrbor.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gwlrzjohm.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gqpllmjev.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gjgpcumed.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gibaeskrl.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gsgbognlw.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gnjrrsgcl.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gikmqrixd.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/goaantyrc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/guvtuxcps.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/grznafmla.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gilezxtkh.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxnxuevzq.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gkhajtlve.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gneyxawkc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gzxpzzxxh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gzbpdwgly.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gjphjmgqp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gdojbjaas.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/grhoxndue.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gniahpyyx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwdgxfvpi.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gzeonhrvy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gutazqyni.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gfrlzeqxf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gumgyprzx.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gzvyowfwq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gulrndvxk.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/grirnnqbf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gecabydyx.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gwzacgkgh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gppwtqhuk.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ginzkvveh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/glguxjosk.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gtjcajxst.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/grjwfdrpe.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gsvoakuea.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/grcfmsbkz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gyeagyzcv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gukppsbhg.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gbbjiqvvl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/golhujlhz.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gfmbjldzo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gyfwzmili.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gmlhcfjya.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gacclbwha.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/glwcydoov.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gqplxkibe.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gqoiulkzh.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gnwrfgjfr.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gsvksvydd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gbzsdnlym.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gmubjizsn.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gyjymgihc.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gunlxvhjk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gujaceddm.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gislyphky.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gmzprqofp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/glmnaelba.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gcldigfgl.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gjuxhdjlb.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gaqabjywz.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/ghkdgocew.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gkqdnbjny.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/grqcpdvei.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gsjfvlpjn.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gfvxwjinb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gpjurapkf.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gmrviqsvc.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gfqjpdmxe.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gwannvyzg.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/guyhfpefn.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gflxwzfio.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gvucdukyr.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gbslyfuen.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/guvzqtaka.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gpgalflsz.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbojphwxa.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gifsfrtah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gxxdrbjjs.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gqfcbzked.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gjhtbjfhp.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gequmxblk.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gxkmucvdx.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gxkpuypnw.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gfrfvtlfo.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gdumvrest.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gjokvtsby.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gmdkethcu.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gjjjhjeaq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/ghwawmlru.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gkyoxjpfy.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gvktutrzs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gtusctsyl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gpcyamvky.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/ghliaayou.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gnteoquai.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gmytucqhb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtnxghkry.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gifjkvatw.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gsibdlkuf.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gfvceftwf.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gdafanvtw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gdbdxwyme.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gdxrmpprp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gfgnkvvyj.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/girjluxqx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gqhntncag.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/ghmjhkqsn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gplvyxtvy.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gjhinxoiy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gmrugfgmn.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gjzqvblmq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gorwfdqzm.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gtaqqvjya.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gddteontv.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gvqncoxfn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gxgmfawtt.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gfamplyig.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gwkjchqab.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gcvfgzwpo.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gokjmkgki.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gatfzpgiu.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gejpbjfpg.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gsrrpcyqi.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gdramciqw.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gtdxadjfb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gmkaqbhpj.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gpqfgtwna.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gtosbzwfr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/guvpwctnt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gszpgfxdp.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gmgnpkczq.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gswnrhxtm.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gugpwwduh.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gytpgrzeo.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gtnkdwnrh.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gecnfscvv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gbuxkqfuy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gsmyzmxhp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/galfsbwxc.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gtvopzylb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gonnwqijc.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gyxyywpqu.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gfluootkr.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gpqfjtexq.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gowqkymck.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gbmroxfmv.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gvgtfazjp.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gsqtdsosv.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gtihollem.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gelcsdevj.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/geucakwgz.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gxdgfmwyt.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gwsmwjzmr.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gazseyawn.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gbvusctxy.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gretmfcln.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gknbkogxe.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gnvpinzne.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gkrkwvaza.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gfcprnmbr.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/ghpxrjqbx.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/ggjgjjnts.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gvcrwjouf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ggmaxvhws.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gehkahklw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gqlumdyuh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/ggjuomqvm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gcawckhmc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdabjtggm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gnizwekoi.sHtML


<!-- 参考信息 -->