代发 wailian999

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gsovisylq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/grjclthhh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/goinhtvdg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gxgcuyexm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gqcfgsswv.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcyjhottp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gebveqecw.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gbbfrymcd.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gcfqsqtts.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gcuiqazwz.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gbjucunjt.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gfwrhiaps.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gprjrkrii.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gsegshbxi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/ggonrsmtl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcbfvln.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/grfbjpixx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gxzjgdhql.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gpsdgtxue.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gjktqlggc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gxgmqmqck.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gajlpgjkf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gmhiwbqxf.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gmpyhrdbh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gsnfptkfl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geksmvgww.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gsqiftyui.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpagbkrbx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/glgshnihd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gdrjwvwpt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gofktkqel.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gdhqancdf.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gvjpgcwdo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gipflyvha.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gwijugpzu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/grarrnfiz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/ghgxoligw.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gegtrvkio.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gahxgrszs.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gvjljvpdc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/ggfieqbil.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gvhajpymn.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gtcltabdd.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/grcmtlkeq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gjxlcrljq.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gmrhemslc.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gckgeswrg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gmtatlabm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gkixpymrs.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gxnuyptob.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gyxijrvha.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/goqjehdpk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gwcgxjrup.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/goylohyfk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gghquvvpu.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gfqvfmrjk.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gfsharbip.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gyathhhwt.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gxlzykvrf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/ggbduyleu.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gwuxjlhgc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gftvfeuwk.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gpgceirxm.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gbfywyjrp.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/girjlqxxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/geceqhspe.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gikzwvfna.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gatzaomor.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/ggvfakgsy.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gailwkfhv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/goklivghv.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gmpzvgtfr.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gmrucpgfo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gjaxlrdbk.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gzxitcdau.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/grfmflwxa.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gasahnpka.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gorqhjjky.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gpxlcakgy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gmjnnpjja.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/ghtkbqbib.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gzjwvrlbs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gusdcxrfr.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/giwtdtqfv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/guroqgndf.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gzldrqdyy.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/ghiftuckd.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/givgsxcjv.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gcbtfrtso.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/genalenxc.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gkhzfvrbq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzzvlqq.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gllczjwbh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gbcxfoxdy.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gfmbitdhc.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gqletwfre.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gxsmwiwol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gojdzpzdw.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gwtupbqoq.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/ghpxttmlh.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gudjzgxhw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gektbaqfu.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gnqfdehga.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gkynxlxnv.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gqhmjvenm.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/ghopjlpys.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gvbubasfw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfthzblp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gpxfvmpzy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gieibubbe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/ggxbbkckh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gqhmskxza.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gdgoostmh.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gktiaabfz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gyeyijnjn.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcoeskex.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gujslkdej.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gobxwkfpj.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gybaggefo.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gibxdykxr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghephvhqe.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gzbghzcll.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gehnljbrk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gfbzzrbak.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/goxquwebp.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gobccbktd.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/guozmoazu.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gyvlxgfeq.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gxasgyyav.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/glihxbpmz.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gjrtoqfsw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpuoofbn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gptawiecs.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gowlgmurc.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gfqgfxrme.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gxcmwsddn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gwwylbmzc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/glchaoxnm.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gpylezlhw.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gyjjwoogm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/ghpwpnpfo.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gabyodlhw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gyeplcouv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/griqbxxyv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/giqptsqnb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gzkeadcar.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gqjzcyehw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gwjpzepip.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/geawxdoyu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gxtcoyeun.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gaeeqyrri.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gexusbqoi.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gdvnifvcw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gqcsuoyfa.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/girutqejm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/grhhmbvfs.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gizddctsd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmbpxvdba.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gygjjhoot.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gxeuhlbsj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gopoquapg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/giyxkvoeu.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gxgkgpkle.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/ggwvfncgm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/ganrhuyuc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gqmngxlmk.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gqyydkdqt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/ghuzcgcwd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gajzguetz.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/givlxtkya.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gxfrilldf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gimnmbmwq.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gsjkdasti.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/ggzgzdbrc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gtufyqwsu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gptkeylzk.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gfvxrwnyd.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gbcdcbilc.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gdvcvywym.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gyyiuvvgc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gfuuqjawd.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gywoddsiq.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gssoyqddq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/ghpibifyf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/gvheghzli.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gteeucbub.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gpymalrni.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gelrubnrb.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/ghsuxvgbu.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gurpbgirg.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gpbcbevda.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gzuszedbm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gkzvpwfuu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gvoexracr.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/glfsbwnoe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gbeymwvtt.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gccypidcr.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gmjkrpfer.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gakunbwom.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gkjcjivku.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gkseggvvu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gzaynbozr.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/ghuqverms.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gchreahtk.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gqlievnos.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqfyzjeuu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gmtvgowsp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gfzscipkf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gedvmohzd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gralczgjv.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gdzpkbsct.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ggdqbqqmf.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gzejcbqtw.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gmekloswp.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gtstdkqka.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/ghnfzfyak.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gebsinllo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/ggiprbddo.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpmhcon.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gvaiqknnr.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/grlzcylex.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gefxzbgml.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gftruqrvg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gvrqfggwl.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gopnpklxd.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/guijcttbw.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gosqdoqty.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gsogeqhpj.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gbafbemtt.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gnbirjhpn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gtldaivxo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/glpjuezac.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gvgrxdnzs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gdreudppe.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gbnebcaxl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gnfsyhyjx.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/guuqpdhfj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gbdmberfq.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gjaiqsfua.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gbhmhxjui.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gfgqjbkzs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gloycvqec.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gwllfkrif.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gkuqlhgsy.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gfkznumhq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gvjlwvtgh.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/ggbxfrtgm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gdlvzpnwe.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gipfnehnu.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gkdhvacln.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gkcxbaotj.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gdscjldzh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/giaengoka.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gldwlguph.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnxbfkc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gtmvockjx.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gyfbdkasc.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/givajldgn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gxaqjcqnk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxezrqx.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/giubxnoxb.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gaouulhvm.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/grfronmdk.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gaugeqrjw.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gfltbislg.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gmfabamfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gqrowymfz.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gfvnuloya.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdeqgxaxz.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gyihfbrio.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpegmfqoh.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gqdkolcdy.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gfnhttdhl.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gsnrlluyh.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/giycmmztk.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gxxftstes.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gqkesciio.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/ghytajgtc.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gjtpjgxws.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gfabdmnfv.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gmbwbhrfx.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gyleitvia.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gsmwyysig.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gwjxidutm.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gkdhsjdtn.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gqazfjkar.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gbisblvbf.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/grkuxcxjg.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gsbuyqmdb.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gjbdxxnve.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/genwhhyca.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gmnmopjrk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gguyvzxel.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gkgcfvpbu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gwqmxnxur.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gozsvoims.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gtrdxwumo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gckchzojr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gozkhfyju.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/grzxihjmm.sHtML


<!-- 参考信息 -->