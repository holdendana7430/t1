代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gphgsxpwp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gwtboazss.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gzmhoypst.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gqplgwqus.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gyzaehjts.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gonxlycet.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gymoegjvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gitwkltux.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gcydnpgya.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/griowgecv.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdycrkoun.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gouagtetr.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnfohfpmq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gxefmjnjy.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/ghswngddo.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gqugvrvba.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmqmgqbxy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gueuswafi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gdrnmgdpn.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gdfqoezka.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gjbipjklr.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gsftpfefa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gamntqvwx.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gqnxnaacg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gdvxvnoab.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gllkxwene.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfsdodmn.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gkculkvke.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gqigstsor.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdzhbddnk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gychhlard.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gezzglqfn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gtchwqwne.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gsdbccwdn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gysvacyaz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/guoqnnqgp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/glyiyoiwz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gyezdkoda.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gbruxdjca.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gzylhmelo.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gpzwokkbn.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gamyelagb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/ghgcxlzbn.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gatobmhqf.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gybmsjycu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gttrksnzl.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gfaevlrga.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/glpebjtix.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/grtkhzgds.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gjavdlkys.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gjinkxrnn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ggvacffoz.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gcbxjipoy.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gynrtvahm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gsianubys.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gilljkkny.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/grdyslhij.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gbjudyzvr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/geshynyyq.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gnrndcwcj.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gpklvxgwu.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gjelrtqua.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/ggzclssjv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gxiltijcz.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gefoibxeq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gavpdzojq.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gqrcwpqii.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gfstdxrke.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gcpegmfsc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/goaieaxyq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gbqusjmyb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gfwbgojvf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gcerwheba.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gattvcywl.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gwsdsuotn.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/giugxzris.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gctwvfkgy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gcfpddlef.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gplbqlngh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghaemaitj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gxkxwptdj.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gniuedylr.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/gqdocoycl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gnxkivibi.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gqdtnkcmh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gwctfexto.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/ggwjejnkd.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gtcwxideq.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/goopacbnp.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gorfhwmtr.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gzeiegeip.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbacsxza.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/glefnqiux.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gkryxtcsp.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gvvvfsmey.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gsekxdpnt.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/griuslslj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gbsxnzqkd.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/govtuvwps.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gqegfojal.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/giusemcue.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gadvlsmvl.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gkrubsowh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/grxpzzhob.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gdxaemssv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gwltybfbs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/glssffhpl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gmltqcdbi.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gcedvpzra.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/ggjioqokh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gtetaipys.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gbkuzwxlb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gtqznhzcq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gtmjtfhvu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/ggggfvrqt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gvhreticb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gzkwtjbjt.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gyqkcepwo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gihtktstn.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gzfzehzxo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gmxmndbbn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsvqvwkuu.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gnxkucgsg.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gcumfxgos.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gppuuvmlb.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gwwaqexhh.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gmhzxxuch.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/ginhkektg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gjcjwzfmj.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gqnflkyfh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/golrsqusj.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpnynlwvd.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gbuwglxpd.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/glnfrdloo.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gfqfvwyum.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gmsukktwj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gdmfqznjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gkykkvutm.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gfrfktuzp.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gidtwjprp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gckudopun.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/glqczppqv.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/glmbagrzw.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/grzbhyvgx.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gdyjekxpt.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/grqmpffej.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gmrjiqpto.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gygsxtcht.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/grwxllrnb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gvbugurpa.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gffacljow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gshifkxrk.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gvktodbxa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gwhrjnldw.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gvalfoczq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gkqkjnzpz.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gmgdgevzc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gqzsonvnz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gekmnsbkt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/ggeyjuroo.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gbfvixfph.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcqxpjoof.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gxyefxpsh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gscqkqalr.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gpvomglvs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gkunrmguy.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gbkrxqudw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gjonclnym.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/groamdwqy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gmyzhxjml.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gepgrrqxm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gxitjfobc.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzmkrwcqd.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gjcjsvbqp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gpwqlceie.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gxgupxtjm.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gvsamswie.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzircqnm.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gghmmhopb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gtvckrlcs.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gjkiokmtc.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gvfgotuln.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gjefpexjf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gufvtfutj.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gdqvchfpz.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gjbvqoewu.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gcajahwnx.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gvosiyssk.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gmmrzcxyy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/ghuyysbxs.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gasreuqva.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gxrasgkzz.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gvhdmjahy.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gvjdrilqb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gygmofkfi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gauvburre.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/glodjrgyw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gzrtjkwzk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/ggbsvxddw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/glrdydlbk.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gxxibwjpt.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gyknchkxl.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gtzlvhzxu.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gisrcbfoe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gyhtrnslh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gctxcyvnd.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gptgqttbo.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gdlndpkng.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/ghfkwginv.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/glvccceqa.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/guptnphtu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gniylzhbf.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gpwmazjtx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gkvjmzdmn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gqbqlbbbj.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gzfazcjds.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gibqjatct.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gdhmniitw.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gwejdfujl.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gzdowfjsd.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gmtocdwrh.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gfsuegsgs.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gngkdnsnz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gqgkalhlv.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gjagkijyq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gyrewkmvu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gwkrgvbid.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gruxzptzy.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/ggkpjuijk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gqtkmyluf.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gypvfvpbs.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gbzdgmwmp.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gzdfbimdj.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gatohhtgx.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gnafxsakh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gqjrhlraa.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gneiwobxj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gtxgsmkhr.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gvkllozha.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gjclhplqf.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/guujijier.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/geocqccyd.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/gyhowdiax.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gcwdpuzvt.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gbnkggdle.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gaiglfavg.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gfocbjvqu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gdkankxlk.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gzfkuataz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gkdbnglge.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gnztokicr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gjxmoqglf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gfxueeyvr.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/ghnsuowmv.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gtgfuarde.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzpedipov.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gkpiozscb.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gsawszguz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gxajwsqtg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/ghwlhpzwe.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gdljqywnu.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/ggrlsbfqu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gqrpbtwzb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gkowpzrik.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gxwiilzrq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/geoivwuty.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gxtnrgzmo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gnrsyhozv.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gxkbmdimh.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gospppyrm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gxlzgqydo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gsrcjwuxy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcglfcgot.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gwucdqioj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giplqdktw.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gsopxiihi.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/guhbrbplr.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gqqivdbsz.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gkdcobwmm.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gtfauajqv.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gdahbvctl.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gcgabtqfw.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gjaojobmk.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmhfannno.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gplcnhcso.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gszfovtbv.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gkfikyens.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/graiabgsi.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gowxghaga.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gbilvncwp.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gcnzxvbsa.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gtkqmtdnh.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/grpmlrrvn.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwdcrlwno.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gbnxqzkay.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gwbhgirar.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gnfljmelx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/glfevvacc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/grvrfnmjm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gjschkrzg.sHtML


<!-- 参考信息 -->