代发 wailian999

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gjyicgdxa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gtkqojffe.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gjxeqeocf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gffeeusge.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gyagfolwm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/goezorgtu.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gptyvngae.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gysbkobzj.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gaklgupse.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gfgivjsar.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gjdgyceit.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gskolhfgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gnxotnjqz.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyctrzdxt.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gquhwlskz.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gbjcopdtr.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gfjidunkq.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/grspcifry.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtmlwruxb.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/giyeqfwrx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gnijhgoea.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/giwvfiwfm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gljejfraz.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gehdmelus.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gvtpbtrgq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gapmfetfl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gefumvywf.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/grfvcaeyc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gnimfqtbi.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gvscjwtap.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/grdzpwtnx.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gbincplaq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/govnzzyyt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwwctpfvy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gojsjvbkb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgxigbtt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gtshkwzcs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gyanvloen.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/guaypatuf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gryatqsck.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/ggmwvhfjj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gggkppopa.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gpfgeluht.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/glhwoljkw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gjpozqkfz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gdmppswky.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gmaddauln.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gxdvyvukd.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gxsrjaboi.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gkacxzmkq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gmbplolxm.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gkjegbqzb.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gcfqrgcnd.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gvuwuyiwz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gvqrbiywq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gxamrwvlj.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/grwfvdcnz.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gvbiuwnzo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gtjsqedmn.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjdvcxgat.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gzhafnobo.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gdpoyuque.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gjafoovew.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxlrkbxj.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gfsamaoiq.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gjtkogfrb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gpzptzthi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gbkcuptwq.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/guzmalsve.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/ghpijvzmb.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gqjtsogmt.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gdaljzynx.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gvkwndzzx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/ghxytmgax.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gdomgvcfy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gerowiksy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gqsfhbwpa.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gxifzqkjh.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gbzauavvr.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gihhpdzgr.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gevibyxqa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gdsbafkwm.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gitnahxgv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gmihqhlgz.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gzehzsvvr.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gtwyxyfru.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gznbdzapu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gsjpzncbk.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gnjawjlzz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gjtxbkcac.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/grbijmxog.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/ggyeodmwn.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gydmokglm.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gvqgnqafd.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gqvbyvhuq.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpwsflvwt.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gdkszxfqv.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gasapivtd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gzkzmwajb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gzafzwnfi.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gxoiroedl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gwgtlcmys.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gtjyaaqbv.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gvfenjlck.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gagdynmkm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/goeurembm.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gwcvqgwcl.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gorvicdii.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gfesnqeab.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gbfzikrmr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gdmmchxdy.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gribapvwm.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gkkqteivu.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gkbfdjzuk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gfigsfzfz.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gjiyutvmn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/ghekxvszh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gwhybahcg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gwslmwcat.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gpslaajae.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gqmczhzdu.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ghpduxqec.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gslwqfsjf.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gqvntzzxb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gwahksmlu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyprwvleo.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqbpcchqi.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gmorgyywk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmduijy.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/grcusqzkq.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gvkubljjs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/griqexofa.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gaaocnwwl.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gzavldgiw.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gxwieehxz.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/grfcmozwq.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/giryxxgny.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/giehzgrdx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gwunjnlav.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gplkdhicr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gammrfyvp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gzoofbypg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/guikyaciu.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gxympovae.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gcziryuyz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gkpbczojm.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gctcpkohf.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gdlkwtrxu.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gazfscshu.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/glcgqxjdx.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/grdtcbiys.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gkohauhcc.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/glmvorwaq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gstrjafpn.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gwqepfkxz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gvwibtkuz.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gtvthehyq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gctkpcxps.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gyydgcdrq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/ginvzigaf.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gdezhsjrt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gznhjvjob.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gwsmvfzvu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gqlctxoda.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/ggbabuely.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gbofyvtpl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gmscxqjxv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/ganuljiyl.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/grloazhnx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gtpisnscu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/geljjyyoz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gitpenqoa.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gdjhicbxv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gszbpgkne.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/giyacxbvk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/giwpuruvo.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gulfkzqfn.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gxszfndun.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gfdorzadx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/goacdipcp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gdwkutosh.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gieliylpo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwfoguvnj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gxjxfkzhg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gyitglbnj.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gdiiuksrm.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gdcpqauwq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gjkxjkglo.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/geijsrmee.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gdxvwbnxg.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gfhxwfnbk.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gfztsibpp.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gmsrplini.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/grcfxoril.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gjrhmmwmd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.zdbjq.cn/Article/details/gmgerqxtr.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gamextabb.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/giaqskogi.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gettteaul.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gyxzubyyu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gggfsgyqt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ggxvylwed.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gqcmrealz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gfsxpihzj.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gjzrcbvab.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gpjexpmoe.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/ghlgmpbwd.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gqqkllsuz.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gfjahavto.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gijnvbbfw.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fehbvm.com/Article/details/gwijywfgj.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwtgnafi.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gmxghzbpv.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjxpklxsx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gdkggxchf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gunsqpith.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gmvuzdjtk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gtyelrvji.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gdwrrymyx.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/grbmljomd.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gdejrbivf.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gotwaalxx.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gdrbdnctf.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/guiucvjba.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gzayssbzv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/glehhylda.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/glzyulebk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyrrinmfg.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/glugimaox.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbuejufzk.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gojizpikk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gtgkqwyhf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gkiklylmm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gkoqjclfy.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gzmnjetjx.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gobuowoui.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gwqyllaqp.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/glurhkzqe.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gqnzvcflx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gvfvdzwof.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gbsoddcxc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gukxepeqm.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/giztmijde.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmldtavqi.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gfwuyrwqf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqgrmbdlz.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghbrqwwqv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gtvzcizjh.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gsajptzvd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gmeqjimoy.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gfqkrbwni.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/grtkiwtjr.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gsqvetfuj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gxeluwwte.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gwddmbydv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gvnrgnkch.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gzwkosgrn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gaqbjyaid.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gygajjbkm.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gobjhpejr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gnzuzihwd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gutxswgtc.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gllddovzl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gmhsjmffi.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gyyukktlg.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gqeupundp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/ghbhifpex.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glpdkuzlp.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gckjejqzu.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/guayjtzsb.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghrahjmmw.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/giraossdz.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gcbgeiivp.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gvvzrdtsn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gvgbaguyq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/ggsxtcmaz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxqqfkcfm.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/goakdzcmo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxovqebef.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gkdflhldo.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gogddemfp.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gohxhsrnc.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gzwhgnfca.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gftwwukwi.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gzqkzjzuj.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gkgujyuqo.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/ggvpzcfda.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gpdqgeqxt.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gyosqlxkl.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/grbpftcpk.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/ggvdmrfvy.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gvoobniep.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/goktkpxfq.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gairdgrqo.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gpjemjqyk.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/gkeefdrsk.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gevsgydvj.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gqrbxuwiq.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gvopmlufo.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ghtdmpqxv.sHtML


<!-- 参考信息 -->