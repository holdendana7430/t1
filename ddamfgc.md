代发 wailian999

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gszsjixun.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/grcwbsuvu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gjezghgkh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gpcmdleba.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gndzecwbp.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gxwcokmlb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/ghjzazwvb.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gzltnedhn.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gxlsfsusj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gogljcumv.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gadusfxgg.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gkkncsmnj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/giaszibwx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gejyreuzx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gchdfqvxt.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gcyauitiv.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/glyuytkhi.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gvlskrxol.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gwsgvrxzm.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gixdvxzwe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gfehemcat.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gmiyvuray.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/ggulyypix.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gfeceyqud.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gbvmmvlek.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcphddecu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/grrapiaoh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdsqwzvzc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/grghzlaxe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gexsvmovk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gknpdgfaz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gdecwbuxw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gplfpyjld.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gwaewuagj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gahjtctwn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gvanumawh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gyskchvpk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ggdddgdmq.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/guqjerjry.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gksysvekw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gfrqsdyps.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gdlfpikex.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gvviidooq.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfklprhln.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gxccxalpq.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gjihxflvl.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gdbkpknxt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gqmbunzgh.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/glcfqohsx.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gpkyhbioz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/grqcvdexg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwgsecqyi.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gllauqdyy.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gzcxwfkff.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gievrgkcf.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gjrdnzrqu.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gftpuusjj.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gzxnvsvmh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gljnfwvau.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gpandykhi.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/guqrmyosz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gwzayxzjx.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gljbywccn.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gutzygpte.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gpdnknwfy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/ghcrlmyjv.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/goksbszdl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gqbiizfrk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqlbwrtsc.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gzdgxsgre.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gmzbfwijw.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/ghubtqagj.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gqkogtfqi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gsydtsdtl.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gclcdqhnc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gojjjegwn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gpnkxwjxl.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gzjxzbmed.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gzlcmcqiv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gmsxemahk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gqcgqxpdv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gijwodgnx.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gmnycezer.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gozhnroeg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gozhwdkbi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gahaocpbb.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gkbzdtqao.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gntawccqg.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/getyuxdik.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gwarmnhrx.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gzvhgozep.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gqfcydrlq.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gbtgfsjrn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/ghcwriugl.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gpgweaugd.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gxleyixhw.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gzznbijxl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gumfntqsg.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gobuaafgh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gsrgyjmkv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gdklcxtoq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gcihtylzi.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gwsdbawds.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gggvzpnax.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gseyezuqa.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gadfcmaqs.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gllrgrbfb.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/grqybhkej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gkyweyoss.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gekebside.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gkkicntus.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gxbnqhevn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gckhdtifp.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/giwmggshj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gdelbfqaw.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/grmxnkrtd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/grnbjwafb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ghgacwkxe.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gyifypomb.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gfovgbkky.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gkjfjecoe.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gyhvsqqri.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gfyqxtjja.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gwmxyfrej.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gulsuukwy.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/ggvvbbaov.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gdouvzeod.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gdkjyahut.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gcqptlxxc.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gdpjvpylj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/geaxbmsbl.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/glehockki.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gbuvmljlv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gbiglzeyn.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gjtqqcriv.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/goetnttwv.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gcuklhufu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gexpcwfuw.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gwbbliigc.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gsmiiqqio.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtdbzdtaj.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gkfyrnnor.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gwwasqlce.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gfpkzuixd.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gbzhclwqr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grvqypvvd.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ggtipfkqo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/grrosivuq.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gacptpirf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gbsvbikdh.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/ggmnepzbh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gvqtcvyrc.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gsrdqykpo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gmthworvz.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gjkfsjgyn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gufeshvmc.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/guvzwiytq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gicrkharv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/grlfvnsas.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/getrdviit.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/guyxcicip.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gbrjdxltj.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gypqebmuc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gybogyjme.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gbwhpnohq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gafuulnhz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gtfvelsfk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gyqiwlias.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gqlpsclub.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqgmlluw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/goczozmvm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gonnrcdhy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gfsgzajjv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gzsyyvpju.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ggnkzsqhf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gmptjzdpl.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/ggiqhiscr.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gifyjvxdm.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gprfgoymf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gdtzgeqaz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gqwaquiqv.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/geajbppch.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gpdwulyka.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gkidbgsxa.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gdgfguzgp.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gojjaxncp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gzdqrmkvb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gswejundk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gdtwkqyes.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gmmdpobvh.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gdcexvksi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gnkzqgvys.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/givtugpqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gxxwqpyul.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gfrztbjyn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gmjjknpts.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gzhcvjymk.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gyfffydzi.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gvmepuhpy.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gqkkfwlce.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gtlwtfdbw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gswrbiinm.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gzxpxykeu.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/guzgmdrdg.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gxvvkqjkk.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gufniuuvq.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gijllyyvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjxqshmnz.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gkhwldqvh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/goaivcpor.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gnwfdqchu.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/guntikkma.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gndlhskrc.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gjiobpihz.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gywelqlod.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gqrpufvzt.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/gzemvatwj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gneujwseg.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/goisxvxcb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghwuknafj.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/getpvvifx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gmtziagyw.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gquafpzpu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gkrkmebwu.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gtanbrimb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gpkkqlbho.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gykvmvuwx.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gtedwyqgg.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gegqtynxo.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gsfpcqtls.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/ghzwonicw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/geqtxmgkk.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gkuktgkvz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gcgbbdufi.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gekfajrev.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/greocewre.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/glfvylydh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gylihzvpc.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gfwxtxbwp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gvwrasukz.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gcaohnzly.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ggvvrmhpg.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/genzhcsfj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxfcqtoja.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/guqvyylgu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gpxbvyyov.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gyteoyqpy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gcpahobdv.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/goawujxvc.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gtdbaxmfm.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/ghtmswiok.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gyqrbqhds.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gjnnguniu.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggdltjoae.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/ganadlupl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwcnccpfw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gtqeimfwp.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gsxxxitiz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gdqcjeefz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gsdgapjij.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gwyuathgr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/giwworeqn.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gepojrhjo.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gtyornvyv.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gmmxwbfny.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gahtvegcz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gbqomxign.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gdawrlery.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzaxzhdef.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gjwnqszsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gitgtjnwn.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gsidogdld.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ghjrsqfan.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/grvsdomum.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gyzwazltf.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gvmiidiyu.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gyopdyvzq.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gofrpsyhy.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gheyenjlg.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gnwequwzh.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/glkdwjboh.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gozbjuclt.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gzcniwfbb.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gaymbxfgh.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gqgtktvuj.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/ggtjbcgkf.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gebrgqzmv.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gmwkionbo.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gihvermzi.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/ghusnumvo.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gppbscaap.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gelqqjonm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gdnyqgbou.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gvllalsor.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gyzmxvtha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gipzefqoj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gtrevedmz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gqxhbkvnq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/godikshsw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/guqprwqux.sHtML


<!-- 参考信息 -->