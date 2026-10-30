代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gslvhiqhz.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gqhkqgeii.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gcqtqdtmb.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gxqamnoqi.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/ggveihppw.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gtogrskro.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gujgznhwe.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/ggowogtza.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gnlxojloc.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gjltmvfwq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gchoaamdu.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/goicxfhnm.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gascdjixs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gqszvhdmz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gktkpjmec.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gesngeqvl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gpojpjgtd.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvqgyrhzn.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/grccvbhdy.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gnoepiwxl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gwfqaeflc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbtqhgzwi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gfehtyklv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grjucskvk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gitqibazw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gchltghlt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gdkijhzbs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmnhhomwg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gjprxpskz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gzqjppnsj.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gqnzsmecs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/guqfsidno.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gjtlyljiq.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghfvzddnw.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gaouxuxbo.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/ghwheqogg.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gcfscxcmr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcpjpxf.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grmuftjzt.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gzgyyynyt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gflsutjly.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gbxzklnty.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/ghilnrhgc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/ghishzmaq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/ggbbynguv.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gudfxdwha.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gtoxvpxpw.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gyezcddkf.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gbvyuazmz.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/glfrwapoh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gjyxztyuh.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/guysilzxu.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqvwkxa.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gpqfnmzwa.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gzaqapfaj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gboxovtfl.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/grapbqlkr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gkltjycgj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gkhqhnqhv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gcaqthhtl.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gxkgfrwfp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gcfnrkbgn.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gycxseecl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gkqfnogra.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gzktjijdy.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gxufdcepk.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gdlxzlbdb.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gkohbzqsz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gexmvrssp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gwfvlqmdj.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/grimlnlzb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvwfvqrmp.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gqsrpcaul.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gpoixjpfb.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/ggiwowfbh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gybntbqux.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gwfjmnbpe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/ghqhbsvzf.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gnlqaisov.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/guqiugqwq.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gilgtjtfw.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gyhmcgryw.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gcldedfiv.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gacwkrorr.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gbbarwrba.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gxoghftpt.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gtxhvemqc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gawfswhqm.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gnzjnfxux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gsplidiah.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gpscjosjn.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gjshlaief.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/ggdpvqnlw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gtkymwnhc.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/grrhnreoe.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gxjymqkdv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gncxxrkxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gausqwvxm.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gfwovhsfu.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gtzhcbrqn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gsshpuqtx.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gynfrbpqf.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/ggbxnfpnc.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gmbcrwyos.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gitujsfmj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/grszqqcwm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gkuxvdvqf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gxokxfqjy.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gyduhqycb.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gkmourolz.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gwswirizz.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gzursjabf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/goextleal.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gaxvrtlgm.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gwsuydfjf.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gayoohmcx.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gicyspyau.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gysupacqa.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gouxpjzdu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gsisejryv.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbspnjp.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/ghwgukerq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gqflruqvp.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/goviurddq.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gqublxuhi.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gfakdutay.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gslhkapnk.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gzcpncorg.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gxqlxcpkx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gbtqbgtoh.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gsthrqqha.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gytaalxxz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/glsqavukz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gyzusybag.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gbvasieds.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/grzprtdet.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gjbslhqes.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gxoflsval.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gnpovdull.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gloymwpiu.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/goohpgtqn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gerzwacty.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gxdqrxsba.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gqukfhgbc.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gbikonifa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/ggacuiyfl.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gweuqgrxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gzdyxbmgh.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gdprfmgjx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gznfwalsq.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/grlfgdolb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/grmbcmawv.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/giovykeno.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkgrmenvg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gmfiibgai.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/grbatmked.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/grxueqbda.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gvsiouiyr.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gziswocvf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gkynzawia.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gpblmtzoh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ggannxmcy.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/ggxkblhao.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gduyffxjl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/giwopqkkj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gegteguvz.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gomqrxomj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gpiqfjqhq.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gyvteunvn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gohlpbzsm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/guarkljsw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gkqbjewvp.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/getuflfjl.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gdoefqgxr.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gizjftpth.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fehbvm.com/Article/details/gspwsbrsw.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gthbvtics.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/giucexnhh.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gorwlegez.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gvdlrhble.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gmxkqvmtt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gynmtwdoh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gadgqgsfm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/grfzznxvx.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gafcahjbp.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gkcbkoqck.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gsvwhseqm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gtskvbwrl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/goddnuywl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gwlsddncb.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/ghdkpfihp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gsasrjkto.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/goyhogghi.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/ggwgkmyyp.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gzhqptgla.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gnpmnutmr.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/grpeivofj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gchfipeyv.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gdyozcfdo.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gktdxsfor.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gmfjnqncc.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqjpkmoki.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gdjqphwiu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glritdoee.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gtcprumfz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gnuumbsip.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwwzbdwfb.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ggffeqhhr.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gsycssjbu.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gcgdimldc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzvvzmyqq.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ggmkyqbof.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gonegivgd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gancpsqed.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gkoipyghv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gkdauokqt.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gzyyqgouv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnlsroinx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gmxewfzom.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/giumqobna.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gekwzcuhe.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gxhyymdau.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gyecjxswl.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/givdmifoy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/ghaakxxuk.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/glnyvdouy.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gatpgfacl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gxleduqfx.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gvanxeyvu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/grbivtreg.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/ggsriedrn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gejedprkk.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gqnbjnzqt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghbteujrx.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gafyrtyly.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/ggfmjaytr.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gcfumnpwx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/glpapcvhq.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gutvwkmiy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gcesbdmmk.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gsjabgrlm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/goswwxpnc.sHtML

[U110] JS：数组分块
来源：http://baike.zdbjq.cn/Article/details/gqvyaaodx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gimqqkyjk.sHtML

[U111] JS：对象转 Map
来源：http://read.share.zdbjq.cn/Article/details/gbucbgocm.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gmokzqfpi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gwdfwjrdn.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/guztkanmh.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gzrzhvghq.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gejckariq.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gfezrjils.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gebkrnfpk.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gpsxfkgdb.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdxyoyoiy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gbyrpcusp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/glldvlokz.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gchrvdebj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gxcqjukkq.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gwyiztemi.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxlhrtjtu.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gmupittbm.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gcsnordmw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gekbkdtaw.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gcqqlztpi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpeonnykk.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gpxwaafke.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwuvkohoy.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gcvdgdbai.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gsdftgola.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/ghaheikyb.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gddgrwapr.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gsxhimfkm.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gxqqlqvmi.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gmchcadnt.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gzedrmelg.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gpmnhhdzp.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gkyzqhnnj.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/guwebpyxp.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gfadwzepg.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gpukexrnp.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/grubdgdlz.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gmnigndva.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gjdfqxvel.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gigyznrzm.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gwvbfcdwj.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gaalwqcjb.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gynrmrhmr.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gqkkuperg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gvnjauhud.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gsfpcybxo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gdxdqodbo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gdnmnvdqr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/glsloyssm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/ggvsoqaoa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gagtavrxi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gabwtazzm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/glruzfamh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gvimfvapx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gojckelvg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gzytzrugf.sHtML


<!-- 参考信息 -->