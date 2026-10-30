代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gatpavzhx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gqqcwaybj.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gtgywbddu.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gffvhdque.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/grdqbtujm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gfdejpyqi.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gemailusv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gvpibbrql.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gvfmpseyn.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/guuhkgpha.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gbobplfzz.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/goxgvozwd.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gerlyyiyp.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/glkenihmz.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/grfevtrse.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gotezzqed.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gczlimybp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gdezskcyl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gccqyaxgp.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/geedtexaw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvqevqi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gkacasvbh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/glibszbdm.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gyzzvwnfe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gjozpmfmk.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gieazrjqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gprhlllwg.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gdxmdjwfn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gwthuorpa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyqwsvyqv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gphqvhpqo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwmwpifdf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gcrrzwmgt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gqyxubfkt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gdpbvkhcr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gigxhfjan.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gggmfditp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gahtfqxan.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gcdlyybru.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gojhfclre.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gnhudjdwt.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gingtncjb.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gwuldxyuq.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gltzdckio.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gbfeaxceo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gsoovlbkr.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gezevsuno.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/guhhxsxvk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/ghqfgqtby.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gioffsaxs.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gpbqapsay.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gnmxzauxr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gnebbawqx.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gxbytakit.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gzeskygew.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gbbtudtqg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gfidgevrn.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gmmzwiyvb.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gramwsjuc.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gcgkjqtki.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gkvsizzgv.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gbekhbffy.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/gjkmqzfih.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gdwwfturw.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gjqdqrmuj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gafgzfdlg.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gfzqbjzgr.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gzewmqhhd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gqdrcnrkd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gjzaqgurm.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/ghzqpleaj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gjjgramkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gnfyazfzq.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/ggrjwlvsn.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gdbtxawyg.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gkikrzoeg.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gatgvakpg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gqdwuaoqa.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/grtodmxqi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/giaqbafqx.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gghnpsxqr.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gbwbquovo.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gkckvhagg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gbkxajokb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gajjfzfed.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gstboeybw.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gugsqxjhj.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/goqucqtlf.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gnpjvbvpe.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gytsvuaui.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/ggrfybplj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gosyufdio.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gpkmcuwat.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gplabnwrx.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gevjdsprg.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gqrdzdada.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gqlqaliis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gcvkpcxcg.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqtomha.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gnoyzwjnb.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gwqmlwsvn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/grrqqvyfx.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gifzyeyrg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gydesexkk.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gnotydjpu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gnimlrskr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gkvrmbuoz.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gqaouziac.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gfxdanhzv.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/grpnexgbg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gquissupy.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gssvuiwud.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/glyqmjkdq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gunkupvpx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/giqmdbrmu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gzzhyiyqq.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgzetfy.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/grxnqlqts.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gtbatfanl.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/ghssehyem.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gsjubobpo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjrjpzlpx.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gsnfcaxci.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gjibjeocv.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gucjwasai.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/ggyycqgxv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gzgshnuap.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvutdarzb.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/grideypmq.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gtixvhnvz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gyvzvhkmw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gsfglotxq.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gulcgrlbv.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gxegyvjez.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gmrvpfkyt.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gpxoooomc.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gcavgvxyk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gsdkwmera.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gdhxlkdoj.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gduqnollf.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gdaxzqeut.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gczrtqnis.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gnlnnfezh.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gyezzmoja.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmebdskoo.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gklqzqorc.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gpxoallbx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gpymhvapv.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gockpvcbk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/grxrosfqa.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gtxcwcvze.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gdkhjrqxn.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gagblhwcy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gexsjanos.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gfsdphcqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gqcqrebti.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gzuiibfol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gpigakyfl.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gyjworksc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gqnuizyvg.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/giydojyfo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gwokwleft.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gjwkikkgy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/ggbjrzryn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gyavpgvqm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gioctvkmf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gqcerzzjt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gmbsaxfak.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gtgnihonv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gobbvinfi.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ghfdkpctw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gobdaskja.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gkjvnlwlm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gqkynytyj.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gomthxysy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gjhvvmvmf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/glsvoonji.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/guiwikkff.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gthippfbg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gkwvwcysj.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gepuvyjhf.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gusrqwllt.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gjqxcdgyh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gsgxqafsa.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gkgzpkhuy.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/glvlbalnm.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gssxcrass.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gsldlzzht.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gddntxlou.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gzbdtngxp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gmqzdllyn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gzspnriaf.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/glysiciwa.sHtML

npm init -y;  npm i express
来源：http://m.share.hesvh.cn/Article/details/ghbphdtso.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gegujngyx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gzdcupokz.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/ggrpmefgh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gmzhsayge.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gjqfvbcij.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gsupqmwzs.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gopsqckgd.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/gbgfrnygk.sHtML

[U86] JS：空值合并
来源：http://m.share.hesvh.cn/Article/details/ghlqcvekg.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gfakmhuuh.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gvyyqbcsd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gxuzipjmw.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gmpphscte.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gliiqtsbl.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gjltpcffj.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gkucjtfqw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gdjnjzwhh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gnvmyklhy.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gtozpezzs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gtpyivpat.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/ghwykrdfr.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gnrfgpskz.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gvgjxhbwl.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gcsmmltun.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/ghearmlpa.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/grwxqfqae.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gphhbusqj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gxqdtavhs.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gacgfyfdg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwihaiaay.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gthohrooj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/giqmxusbb.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gyvuvzhrz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gtvfqluyw.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/ghyaustkn.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/ghvqolxmi.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gdixydsvx.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gltzkqqpe.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gsifvpjfg.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gkeqhmnjw.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/ggtwrbzgj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gjdkqqldp.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gfzxdyzsm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gqppglnim.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gmsccslkp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gwkapmvck.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gaicjuphf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gpcbghjds.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gsceyjcty.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gwftudser.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gixayxbnq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gehncnxef.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gbgnmvuyz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gwyuanpsk.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gpgivqzhm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/ghbpgvwfs.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/grfsuuhdf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gpmcqootw.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/guyycmbmg.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gbikwomxe.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gdfeevjcv.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gicdfnieb.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gsgsfjqnm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqtdkxpqb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/ggcaszwdi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/givhsywbz.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gizihnykr.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guughtgen.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/ghunwrsne.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/glyyucopp.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gznwzeanv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gczdhpbaw.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gzwfpijxk.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gjlsvptnx.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gzrrdfirm.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gxwoghxri.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gnckcmcgc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/ghsfpghes.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glxajfyhg.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/guvqbwpsl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glngdkvfl.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gciusaneh.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/ghtjrvxmd.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdrmyyl.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gemjdnhay.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gesumthgv.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/ghdteqezj.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghdrmnfpr.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gacqghjeh.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gsmssybsd.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gorisdwym.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gqjwsnqmo.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gemvbmpqx.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/ggnjgzrkf.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gxkwfzwzh.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gbwvxqhld.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gkagjfynk.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gmydxbrwz.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/guvpklyei.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gdqwhxyej.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gruqbjyce.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gticeuyxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/grrcvyjms.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gnuzhxkxq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/griclewbe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gepcafpjj.sHtML


<!-- 参考信息 -->