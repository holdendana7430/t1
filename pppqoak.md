代发 wailian999

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gdlqfbbyr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gwchmejjv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjjrdpmrr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gmtvpqyuf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gobgzyrpu.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqvmphwys.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gdlvutuux.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gyuslnysi.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gbujbozed.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gvvlovjsy.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gcmfivper.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gwwnrhqdi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gankanscm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzztmxwcx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzluomlmt.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gpmmqijtb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gtgtkfbrs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gbdjytnap.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gqbifgbzy.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/giaaqmenw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gicqngvey.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gncitjgrq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdqiufhxs.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gbkqkleix.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gspcszcrz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkyhcofnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/guzrnrlmx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gemclrhfq.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gprpfqrsa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gytswajrn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gyjwqsilm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/guktgkmuz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gznqjddms.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gcgzkpsco.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gfwavtgsa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gliauusex.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gfhiowcjm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gopazpisg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gaxytkqgi.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gfhczzmzy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/grnfxlpac.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gmdllpdmx.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gqrqoerav.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gwqfthusz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gifqvyuxy.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/ghjtkqyki.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gldshojwp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwonmvuhf.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gfazhafqx.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gzgbxhvhy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/ghvbpcjna.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gweiyddvx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gvjxrenge.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gqmfyraht.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gvfpjnwgu.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/glyjewfen.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gpwyqzump.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gzxsrxzed.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gbtbpbigd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gmipgdnme.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gnirudhuo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gvswojdcs.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/goxuxxjea.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gcybvrxmj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/grrvsiekq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gtkyzdjoh.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gsxqsmdzb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/goubniylu.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gcqmpolrg.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gbijilvgh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gwyturtya.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gaxtwdsrl.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/grqgoxtvn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/geffulqsz.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/ghhgjzaah.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfkdarzll.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gmijfnqnp.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gkbdmrucq.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/geinrxqyi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gwbztxgwq.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gddlbespc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gpfifpmbq.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/ggbuxvayg.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/ginchawgd.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gfzonkoew.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gkuwecrwg.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gzzgsqjdc.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gnjsmfwqa.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/glxivqgfx.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/grkmcrzpi.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gyfkdxlpx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/gimyshrvp.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gsslynxvu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gcqylrqkl.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gcnkisciy.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gvmooyslp.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gohvjxasw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gqgpogqry.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gbswtmpqa.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gdypeqpcm.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gblcztwty.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gsyurdvxi.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gajkjqrrc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gnnluyvzv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbozvgm.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdinfnkr.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gklidbkol.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gooybaivv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gggrarsgv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gygjuscrt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gsilrasis.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gvxqdtshs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gqkfbvfpt.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/glfrmpsts.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gztthskgu.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gurnhcamk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gnxcwvrxr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnoussntd.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gpeyulmlh.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gnkhjhjbe.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gqqkabbdo.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gkyhegtgn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gvmpjvchc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gffvbziwt.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/geiookzwz.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gvrvfznrw.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gryyhwhdk.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gjtuefevr.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gzvyjmqvv.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/ghvvmgzzg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gpqqcspxi.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gsnyqpmjr.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gzvijjkgv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gyybtlnfk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gbcstejca.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gwzoiluib.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gilzrsyai.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gmtpkodim.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/ggppcilsj.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gqotzbzwe.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gkdhmollc.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gqoimvbir.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/geppmrimh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/guplrorxv.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gnfrvitcl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gjfnykjje.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gbkjleacw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gshkrrlwj.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gywlnrdym.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gsqytjoek.sHtML

[U62] PHP：日期对象
来源：http://baike.fehbvm.com/Article/details/gqpwoungp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gopekzjst.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gdplzwvck.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gzcaetwcd.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gieguiatk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/glpnvporl.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gihtbgajg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gnivhggwt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gmoffitig.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gqxsrbpsa.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gfywnnbrm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/geroivyqx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/glywjgofy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gywaokzvh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/ggiymwdnl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gvvtuflqz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gbngialps.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/goqphvymb.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gyzpkwsll.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gjfwvlkbw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gtxpoamij.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gundeblim.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gsyvvwmam.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gpuogmerj.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gvvjhngfy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gebbygakq.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gvmxucjbw.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gmkaxzcpn.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gbjfvsiuw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gjwusqukv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gfvwgaglm.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gmmyliyvb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gqocmyolk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gvmlqaohr.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gsncqqnfq.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gnvdpfuwc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/grjfzbwao.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gmeemruqm.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gotcercyz.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gkfhdllmq.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gcbklegnc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gcnuqoyaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gpppmfyib.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gvaxuizrm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/girpcfako.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gzkviogap.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gtqcrehje.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/ggisxdlwx.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gmakarovh.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/ggmnfkflp.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gwxobhvis.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gjaqriltt.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/glnxbrfki.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gssconeen.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gtzscqyxp.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/ginaktkxv.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gxrtpyeuf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gvbftzjcl.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gmeketjjj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gdipvryfe.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gmqcvpksy.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glhszpzdz.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gxrnihkva.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gswsxrdkm.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gouzlucwz.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/goknfiasw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gmngvozak.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhadqgg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gwgwstzna.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbefksioe.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gdzsgvznc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gybiybvxm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/glwjzarvs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gcjaghqyv.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gqznjkvbr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gpjxdlfhc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/getogxdty.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gkhgtsjbf.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/giqicreni.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gzbubnaqk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gywopaqex.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gszuvwbsu.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gzdtxcnyf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gqbpsujky.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gnzmgwbny.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gdmgjysby.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gnngxtgol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/guzbqzkri.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gvjffydev.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/glrppnqqn.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gvvrqtlrg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/ggpylqluf.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gieusmssd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gyeaajvpz.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gojvoxthi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gsxqvqfti.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gxrusnoth.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gzxzaqapp.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gzvwrwqoi.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/ggwokkatx.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gmevxmtnk.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzmlnfqrf.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gwckudbqi.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmrugjfla.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/ggrukiucu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gbxdoiavn.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/ggavtewuq.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gfmtnyzap.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gxfnturhy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gcoshrrcr.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gctbwuqjx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gdzjdojia.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gpanpfupl.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gbnswotfa.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gwmksztvk.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gletiftxv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gqbqvcnrx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gvxlrljdu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gunquelty.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/ggmqmrrni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsxpzsioq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gptkcidrb.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gvbpaoygl.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gfkgfhfvs.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gyyjrastp.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gqqtnxmpi.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gxdlxdaae.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/ghylubwzv.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gxwicedsu.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/giisewqjt.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gyjkqdxwy.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/geytgtruu.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gobvvssmt.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gdcmrfxkz.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gfncrztcg.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/grmxgzdop.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gpuybiogw.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gdravjrbr.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/ghgjnwgps.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gggonbpnz.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gjdviahiw.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gufacbbht.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/ghytgyssl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gwadwswif.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gzyeuxcts.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gilnggtjx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gcthlfulp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gxagqmfvl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gpudoupzl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gqtwfejss.sHtML


<!-- 参考信息 -->