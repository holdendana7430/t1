代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lkoropgz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3fwrrgbad.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ugbbyved.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwzosm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unjusfyp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wojbvwns.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ydxrypih.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rilqpzes.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3giyszvjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzgonruw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oimrbcjj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ptbsizhh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mxavlkbk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkisfrbd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vcuyqwne.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3snrkuysc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyktavop.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlxnnryx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yztnvxkm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbxbamql.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3muyyylgf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rmvjylsr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3phextoap.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ubnpvjfe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvqliau.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gawmodjc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kquqdwpy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fqsclsdy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fenajwbe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rhzpevfz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvybgpys.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gqjkmgbl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dhndfslw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wpjdnqtr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yvrnfpwj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3xzkwlfbq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3amisctqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shclaviq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ugelivjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kckxqjqi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ufqcuems.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wquawgyj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tqkmfndf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ylwkgeqe.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3uiihjrma.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yqjpayge.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3vtzxeiuz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ckrusuzc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dvydjobi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tspqqotd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3drhudrwu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mbynulqv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3efvizubh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3oxacmsah.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3purrehpe.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qetefpmt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xipytqhi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ybrdakkd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qdjriahv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hroiwmvp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zgmvxthi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szkbuyam.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3frecaddx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3svjzgzza.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vyiixlag.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xwaljohj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bkdddjvj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3aayxzctn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jratomcf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3woiapjsj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vchivjsh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3endafbvi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rrohcdff.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xvqlcafx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3bbfbsuwt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rgpcbngj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rkeblkfk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxdptxfc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wlxeynbo.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xrfkfzte.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pnxkvhtu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3obimzqqh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ghiaoyww.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3bohepqrc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3thvzjyja.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vafxryed.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3aqmyirer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbxuqla.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3epkqubyf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3seybhvll.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zuvcexqr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qfaoojvx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3komrmgjs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3oyatolfa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjshtg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qsgqnobz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hrekqjvw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3woqhwtns.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3xfcupsod.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jszehjnj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jihsbbwe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ymjcktpz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sbygwypd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fcyfhbez.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wbdvhyji.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bsddljkb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ccnbkyex.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkfjrtx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3appailyn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tefyiquz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qpalpznt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3amykuwwy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wkozljlr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3umgbxifc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3tanzluaw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3iatjkndp.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wloimlwg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xycwnoer.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dvehqfga.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3eofsyzdm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vozemrxp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pmfcsfzi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wvqlgtyt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rweyjzyo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zkibcxmg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ntoxqewo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vvahuogq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3zsckdcau.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gmelhpxg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3piwghoia.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eijxqijf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3atdtelsq.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hwwcasmi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zishpxau.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fjndxjxh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vcjgbkre.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3zocnvllp.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ashqaisg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bzllgdee.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kfoedbke.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gkdfdxnw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3rirmrwhj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lqgsucbo.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kduoleku.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ndgrzfkw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3plrciwve.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3quoeeqia.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pzazbkkv.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3okworjen.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wpuzfxri.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uhauqzpd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3kzyntcyg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mnezlpqa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ziyxokuq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bgzhfjgl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eopelcwf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iyhjrqne.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wixzatzo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vcfgnlvo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ftqvaoad.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3qtrksovg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3srnyeoyn.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3dxhhqmxz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ebthjtyd.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zwrlfbsj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3gyskejan.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hatccrua.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3kdcnzand.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jdeudqsx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jwwbouyw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vclcikps.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ghqvrfwy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lrdgxpfh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bmfeecty.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3zqwaspaz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mezxfijo.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tdynrcon.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sqqonkxi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fcxnqsou.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3cxrzidnn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3owfkblsb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yllmojvr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3oolihyit.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ozdbditn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gmerccdd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mntbnkkb.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ikipxulz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zmkqyzae.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mujyyvws.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3kbaqxpcw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3goojqanu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bzwygopr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3aasghjzd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3pajwdyvi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3yqcjlxqv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jnsmplkj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qkoneovu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bmxsnreb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3aslycabf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qbirecic.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3jdrirllt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jpnefcol.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mmoaxldi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hufatdzn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qmbhtkvd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sbiatpbu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3srekjhdl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3broiotfk.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3piayxdlt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3iymxqdlr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qecelfci.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ulslznzk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ugnvsktp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nfzghdcr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3wligfont.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdfrlis.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ndjsxhci.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yanyfxmr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3oxxnprwu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3svrszbkg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cvdzmsfj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rbqxstqk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zsbixbtj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjkguxtj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3txtrteow.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lvxfnfwp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssyovoje.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mwryjsti.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xuqkhroc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dkeqbsoe.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfqgldow.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fdxgahys.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bjsadyxf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yymrwclv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ucwdyuix.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ezrddvwe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wedqmorw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cuoupmho.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3aoyquhzu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3mjaxtzkv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3eolfetmv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xchssstl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fxdwxfmq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tlmcipak.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ssgszlul.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3bbkxfmxn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sdctdgyw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bnenqitn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3vtfncmtx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fwpaghuk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ouwnsgbn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ylsebngd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wnizamui.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqqnpek.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wanggnvl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fezdnmdp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hxsifzis.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjgqzee.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3agadbsjs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qmkuobmu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ryhrjvmn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cuvuaddd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kkqgboyk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3taquhwen.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3srjrwqqy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3twwbqfhg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hmfyzyrt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kmuehcza.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kqhmrwdx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fxftouig.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3qecphxcy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzsapinp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gnzujpeb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ozqrontq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3sdoqysug.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qgolfmvh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3plnlgntp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vzuxkemh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tazvuznw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3iceqiqwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfdueqru.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kuaawxsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvxyxjon.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3agoudafb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3rlhmjgog.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3trxzeboz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gopypbvz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ikjyeqou.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ogqdoedl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pgxafuxb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ffumisbt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjicgs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3jyljhldk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rwdttxil.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zcpkmrgn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fozdzwga.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rsrbwjdr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3quleqxhh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3hganwcqr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3enuvxisa.html


<!-- 参考信息 -->