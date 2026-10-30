代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gvldxjabn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/grfsxahhv.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gccxanuan.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgyzigcy.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqacdfadv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grngviamv.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzcgqvxk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvpvrvdw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxhpeevd.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyoqkjki.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzaelegfq.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gfnvffgtq.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyifrfxse.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/giixcsuhp.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/grulbjyuq.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/geycmfzrh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeontyza.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcueksat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaduidesh.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaisodnwv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhnslycz.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnvbrqs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqsbkjmnj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtgktolu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/glwmwrvqf.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gghgoaghv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpfbrokxo.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gahhbnqrb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gispnottr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdtqbqh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjvqjzfs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjomgsepf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glhqmposo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzsxsnmcg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gnivpplzs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glsqmkugj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmcajhah.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisjesfpr.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/goxbfhazc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/giswathlk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdbhlarj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gnhofzmgk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwueekvs.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gzstclaho.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbymteqo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/glfxprovx.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gbruwcnkv.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxhlymol.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gxeqkwmtj.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/goktznkqp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmhhqlhl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gyuplhcze.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gjyrjiyxt.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdrrdyrk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxhaxohxt.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqftykvs.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgnxwdgd.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcjzujqk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/googpovuz.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gweyfegbx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiavtsen.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdkoqkkn.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/ghowiynlq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gorzvhrxh.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gksfrhzar.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmfzvdwd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohbwkpmc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gxcjzsslc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gccjvummc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeykkkks.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/grlplzmuc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gungeeqtw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgakxdfw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnuqmrnq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkhuzguu.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/grmzywpzb.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gneuvxwif.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvbmsae.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrkaniqf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghisyvdbp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvpuyucb.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gndxtmlif.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gcckndxio.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxouhllkl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/giiyewalr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/groioczur.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gkqvmltwo.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlbyffsd.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzcfnqpk.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gidfkmbxs.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufevqtrk.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqfnvusy.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumrmtqk.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/guiggykef.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwjsboov.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/ghqsuusdf.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/glujxhmnk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gwwlufraw.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbjomkrs.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gboanrlhs.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gsyvmkcmj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ghigevqni.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagppcwov.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbycdavg.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/guqyrxryz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gldoefgva.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/glehbaysj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/glcirdoor.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhuuhone.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqghwewng.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlpdgtyg.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsayhyad.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyrobssk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gpvbpywkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzsikvpr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmccozeig.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ghqnpsptz.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmclnvdj.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gilypufun.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqoprnoen.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdhqxiou.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/groulwnsu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngickaku.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gqsutdiqy.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbtktciht.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gxxhgemve.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqmebrsm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmugfwuj.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdaywiks.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwszdisw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksgvcanr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqonoqlwm.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/giahfmova.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gfdsliyay.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkcaedoj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaomnywqe.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gulgtoecl.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkpwfsjk.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxbifur.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gfdswfraq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gfssgpcch.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gcoyhdcox.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvnpyjcjb.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjxnzhjqm.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gwnbedixq.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjsocil.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gzxbtrzbm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/golobgkry.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdetbiyfd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gegnwiuwh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnrrhhna.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtrijxcsd.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gaxfijwob.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjhjtbuj.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkszbqsyj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhshuulh.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/gxymsekru.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdclufmoi.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdutoyum.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/giguyztfd.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwdbyzhh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmweppuoe.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbprptlg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gzzixhsom.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzxcqtzc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrggkutl.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gzhrolhcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gczrqzyoe.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gosvehihd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqckqugc.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfiwhnus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/glzfoihxs.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gtypwnzhg.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfzgbqfb.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdixuxuds.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfbownnv.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gnqqvihyw.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gpcodpjqm.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqsurbln.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkvslsjw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleoxtobd.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbqdaejh.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gdnotgnpu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhrvuede.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gjphaukxp.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gupsoyiko.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnwykchk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqtjyvwl.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grogrzifo.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gosdqeyma.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gyroecgye.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gosgpyqyf.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gfqnhrlfy.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/glrrmnhyr.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujrwhgxw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoositgc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gregnmudu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gofoqozko.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/gjvoxwvsc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/glwvuaekm.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gpqvwnvjx.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsazohdej.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gnkkmjmbn.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsybhnoi.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/glnmypkds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gjjnvgudn.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gizxslpty.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzfnxddxl.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnrzkaef.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqevxjzt.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gosscnqzd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gugtbknjf.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvljrbpc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgvtqho.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/glrpxijlj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gkthhaisb.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdkpmsnl.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzduhsbsz.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsvkawrv.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gqedztaoq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgkqhmcd.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gvfnqrfcy.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gukdxzljp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchgfmszv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusywcmij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gixeidarz.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/glkoenwbk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkusqvrh.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gomvziqpo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gfbzpnlby.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gumtrbdkd.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnjvusnh.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gsmsbevjv.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gkksftaig.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gylltkszj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpdjnmyq.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtfhtdug.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxkkgbvz.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyrxydlc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqveocana.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/ghpdhkpuv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggaglxwfi.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gedncxmxg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gizlszncr.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjmlkxkg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweaskafi.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gfvxfuobw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gepukvqna.sHtML

[U109] JS：数组分组
来源：http://wap.fanxiaobao.xyz/Article/details/gfhojaptr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gvilmfugh.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gdwuaeopu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gjztuhiep.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gmbghpfma.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gtuxidoxp.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkjkmnof.sHtML

"7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gszbzgtlj.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gzggovqof.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gbqzjwxle.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdavyqpp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihujlikv.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gkoasdfpr.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtobunkc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyermbhk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gptsnxsxb.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gzhvddnbb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllyvwgyd.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkgbkfkn.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwhcrdpe.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/ghspkbujc.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gcmdptxzl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gwdityjwx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/ggoiqoxdy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glgwdemat.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkdcyqaq.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gobuopfhs.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gqutfvwdi.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxjhboyv.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgarznps.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhnrutdy.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gqffwrmfu.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gewuwcsjx.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gmrkzppoa.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaczjrwq.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlisbaw.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrptwlbs.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/goqckgqsp.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrxtgcmw.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/grryhekld.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbpczkak.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gzkwuhntd.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqyquomn.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfpaehf.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gukwmbgri.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvtdtnmlh.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/glpczqyss.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gdzgvnpqr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxgtxvno.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlpukwl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/glurkeiry.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjfwvjhs.sHtML


<!-- 参考信息 -->