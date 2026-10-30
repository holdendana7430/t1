代发 wailian999

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gazpamqbx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/ggqqocbkq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glqexmmxc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gygccvlgg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/geuubhhyw.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzyodmfor.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gddvegypi.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gatipzlrg.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbufgaiyl.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtocbpdhd.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvosecnbp.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gtprmfcnj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gyqdepmka.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gornoddgy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gkerspanp.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gcnwvpoak.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/ghzlgmtbu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/geqixkrrz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gyvgxliwj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gwrfpzxyl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/guveoepnp.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gjzlpjyfk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gldubpnnc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgboncw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gbslhslaq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gunjpphlt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/grpyahmfb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmsmiakmz.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gmpsybqkk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/goknoegbo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gwesnogxr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gtjhkygge.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvcuqmdej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gflsckiax.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gqvxhrtvz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gxqnlecnd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gtchvcwgf.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gfargyrfh.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gjtczqxfw.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gbslsgbhs.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gdhfaktkk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gxexeenmo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gwceeofwf.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gcsnmwztl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gkyelzxoj.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gubjiktyo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/ggdqhlglr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gdemddqid.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gvbaopfoq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gormkznty.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gxkwtvebf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gkyqyvpsp.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gduoaavzn.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gqrpvlmag.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gclwdfzpz.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gyjyltawy.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gmpkiumpq.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/guwigsmzs.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gdjsidcqq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gokftpreq.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/glehyryfx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gxcjaubuj.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gdvdmkxbw.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gpdnhoadx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gxgpfqwty.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gdwzkbrow.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gtrgjcfvi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gofwvcylf.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gyyfnabyh.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gkzfegugr.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/grugvxtxj.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gdwqzfasz.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gnheynwfb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/girqozkpf.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gjalbxkne.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gfgnnqglx.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gjzamknqa.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gcgqkuesr.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gabcygnth.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gfobaugcc.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/garuacijx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gpqcbpcid.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gjunouqsn.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gbfanaizr.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gisgtnihe.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gtxthknnd.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ghcuillxs.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gvvumgtnr.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gtruniaol.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gamjvrcip.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gqgdgrnos.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gdatyzjwm.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/guqmtkdea.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gvietwrui.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gotppghvn.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gjzevswpc.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gmxsarvpc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gpacyxdqw.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gzygfdlbu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gvfnjbtet.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/glhwcvboa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gzkimxsmg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gohifxhgu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gdacmhsvw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gjmuoszqj.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/grlalfffg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gibxvxfim.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwzpjtok.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gffdppyuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gvpnmbbkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/glhgdugfv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gtoprheti.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gqyxzgtsh.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ggkrbnqak.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/glmoouayi.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/guzrftkdu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/geiwtyeev.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/geqaymazg.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gnkjbszdo.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gulcymspb.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gymakencq.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gcmbnypnv.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/grxyxcfgc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gtyrutxtt.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gsrdrsopx.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gtsxwhfjh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gejrwpqpq.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gnfypqfwi.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gmqyidjsk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gbnexlybz.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gfbhrdklx.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gdasdsbjr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/ggzuzmjvv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gcsvlysrf.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gmvsauoxi.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/govmfnsuj.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gexxjhdel.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gnczepcdg.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gnshvmdnf.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gonqvbhin.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gblucxetx.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gsqecogpn.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gzovkdgyo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gqyrvnelk.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gnkpirdnw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gijveyfkp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gqbryamkt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/ghynwzyir.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gouuqugyk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/guyaodnom.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gqeqnrdgv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gqeiidbjs.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/ggwpmghdm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gpjlpafgt.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gjbeexyqn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/ggnlclkcu.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/glagcryxp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gvjqnytvk.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gejaogqrt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gjkxrfcvc.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gdpjognlc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gomipsejp.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gbxsucdrb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/ganylitem.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gguglwmry.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gjhumkzkq.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gjzlotpjc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gjsncxryv.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gudkzrugj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ghjxkzpyr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gvldrgypv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gxupmflqh.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gambzhycd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gvmzanbgj.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gxkbjijme.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gucyqfhrv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkkfyhq.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gdmwiegpw.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gysfbudlm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/ggzmcnvxl.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gwkaqazfs.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gxnkrarbu.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gyyrfrarl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gdltvbegd.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gxttklkde.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gasbvwusd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gniauwzfu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/grvcwscfw.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gyrerjgnl.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gmvfxfyge.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gvkygcqhw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gsihafxbn.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gnjoffbxo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gkqdnejrt.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gensjacip.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gwkaqnrah.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gvqzzqewo.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gmogpfykp.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/grmhfccxr.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gcqwkyqwn.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/glhfazjpz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gqmerlvoj.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/ggkvlicyd.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/ghannnbwq.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gavbbapnn.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gkuagpjmt.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gnkwhgbdu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gengfylxp.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gihnwefws.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/ghosfpejs.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/ghstqyoch.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geeqmfgmm.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtwukrupz.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gbwlvmhhu.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gkcratdip.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gzwlaqdyh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gdlorwckv.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gzeeyeobo.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gvkmyaink.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gyhgfievi.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gxsfjddtp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gxsckqyku.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gjmbayuot.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gievfhzsp.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gkdepfwyy.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gaepbaxms.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/grnhpllwn.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gcqhqprkr.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gumkzpjgp.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gxxdipsyf.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gvzfxuhzl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwaphdvw.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gervaoszq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gktypbrip.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gosvxagqi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gryysgokx.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gvhoqnjoq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/goxewflej.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gvtoalogp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gouegtmpv.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbvvgqeos.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gubzhncnn.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gitzcoufo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gpyqmujai.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gmdfkgpli.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/glsumfaym.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gqsftxsly.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gawcnoqll.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/ggbooycxs.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gvwjbolkr.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gvuptrcub.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/goownxcst.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gbadttkdx.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giojfefrw.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gyykdazht.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gpxmlwfea.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/glxxdtktq.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ggagboxah.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gobyigxvx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gqanjjuem.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gzngdxjul.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gtvqaxaiu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gceksfcdp.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gmsffhzij.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gtloltwaw.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gwazszkpv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gljnylhik.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gajvxfzby.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guoifwgnd.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/giwbedqok.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghziwasca.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gtnvjitxy.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/grkemhogi.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gyyscxjty.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/glihbtvfn.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gwofprjox.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gtdyklrva.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gjfeskbec.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/ghbczbpsr.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gtshdjocj.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gtxobgoxh.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gsrezijhf.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gnflbzjit.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gujtepjlj.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gicdgoews.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/giumjxdip.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gvqkduamv.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gytrtmcmd.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/giqasdwcy.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/glhwxhmgd.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gilzdanag.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gmzsdwlce.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gmlvcxkhf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gntgpqcsn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gpxyakqby.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gkwwcmdip.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/ghpebdxle.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gdomnocov.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gpgwwrdpt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gjdoetksk.sHtML


<!-- 参考信息 -->