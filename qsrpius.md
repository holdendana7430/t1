代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gvdpvubah.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdrvxzrnx.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggnrtcofw.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gajvkaqnd.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gzrwhukpc.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjltpzlzb.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkyzzitkw.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gvqmoatwj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxtmpgotf.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxbpfjhpn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gtkwxzgiw.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gqessooet.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gmujcljvs.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gdywsxgcv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/giszrjxud.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/garafgteq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gjpcwbvtr.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gfdkubmxi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gygijjitt.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gpfwzgyxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gazuiaclc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxifxlpi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gkaxwhknm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvuucqqtb.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gdyixuyzj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gvxbcilrk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gqtvcbqam.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/goabypilo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gxbcdqmqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gpyjvypma.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gvbjmrsye.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gqoupowpm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/ghbqckstd.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gmpjtzymb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gtkaheegi.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/grpidkcfx.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ggobqvhfx.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gfufhryxf.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gyzphtwlk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gcukchlgz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gohyrftwb.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/grheypfhh.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/guvomuxcs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gjxszwyas.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gokfggkmd.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gkohwnang.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/grqncpxgi.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gnrslmhfg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gsddbbmpl.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/grvmqvbcp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gxaqmtwce.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gauqvyaqz.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gnwcigien.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gxblsazjp.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gctrowhbr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gitwehqnp.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gdcaxdcab.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/goeyqyrbm.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gstbokiye.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gvhlcovxg.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gfbbatokv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gqtbiwyvc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gdvjnossn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gscqnmflo.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gbdfbafhc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/guqprenwz.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gmgabndmj.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gridthptl.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gbtedyxtp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/ghjbpuhkw.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gzuvmxbci.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gfynfjqug.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gioqplsqi.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gvaimapln.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gmonoussx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gtohgctno.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/giqrjrnwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/ghzrjykpp.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/ghjesitwe.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gsjnxsdhb.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gkkkylgqz.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gfmsbsgdg.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gexakxtal.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/guwrkifcl.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gzyncwhqm.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gzwyrtvkh.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gyvsvskry.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gpqlwpjpn.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gnhlfpdbg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gjgtklfsq.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/ggpdchqls.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gnxbwdtmx.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gtdcswddf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gtpjlxyyv.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gvqmneevg.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gtjewgdcy.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gusudftjq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gacysupjn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gffqezzib.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gfexbyckt.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gzpibxmmr.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gvzixjinb.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gynbslhzx.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gcogztyoj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gwqqwjixy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gkclmavks.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gsqphalpo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/ghirixrgo.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gflcygohh.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gbqszpzth.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/grehiialv.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gennumbrg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/ggtkltyoq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gytrdqkwk.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gcdtwelah.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gvmtkkvho.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/grewvicwc.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gttkexuql.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gkohfcjic.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggrdudyzd.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gfrhrldgl.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gnsnjsigt.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/guxvyzvcc.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gvgyknvyc.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/goajeyzfm.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gytlotpru.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gitcxytme.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gczgjanad.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/giqmfppvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gcofucemq.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/glyqiwcfi.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/ghtbxxlay.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggufiucum.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gptkrxncu.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gtckpkvtl.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gvxktukhm.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjbitpkvq.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/ghwufpdto.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gxizbufbf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbwhuraco.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/ghtundwbx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gadrfijpa.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gvqawtrwp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gfxxgthqy.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/glayucjia.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/ghubvbddc.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gjbaxpiiw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gkrvrpkan.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gjjgrdhqf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gwltyizap.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gcggkhszz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gtuaspgxs.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gcrqmgunp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grsyetcde.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/ghalyiqej.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gaxyxindx.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gohzblkof.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/guajipene.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/genlbofdx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gngkrnriw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gtefvhnpa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gunsxrmys.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/ghbxqzsox.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gkwrzdnog.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gjrbkgwxs.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/ggdqkzgur.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gsbawgpzr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gwcoxzpgp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gvnbzjgzt.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gdrbwsvqx.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gstroyxzw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/ggulaeagd.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gktrybjnq.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gwskpotqf.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gixdpowgx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gnrqqzamk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gfbeimnmb.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/grfazsazf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gcndxdigh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gcixbjnms.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/grilyxcyp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/ghporeorx.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gmjzejcgi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gzchhzewe.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gxmyrkcuw.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gkualhwdr.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gjfozhtjg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/glkxdregq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gcstvmrmh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gnvvzzost.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gauqblvsm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gnmrbayno.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gncvvetrn.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gddipntzh.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gvjeklejv.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/grxvzedup.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/glmqaifjz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gnvdjqfyt.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/ghyvopshi.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gbzhsdimn.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gwqcqefuk.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gfhkoxgub.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ghscjozmz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ghnomrcer.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsbfymmuu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/geslmubxa.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gudbjogpa.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gaoqpkwiw.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/ghpgxqemg.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gcgsknjrn.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gekfigyes.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gxeagercl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gfcbkyriw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/ghpusksor.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gjmurhyin.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gttldcvby.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/goiixisik.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gczmdutfb.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/ghqopjplj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gnamqiodb.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gggwvsjqa.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gawdyptrs.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gjztnzwph.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gajqmacfk.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gmpxdpxfo.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gyxutvgwa.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gacmzimbd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gxjqnzcbx.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gwkslzpgt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gpywqisbw.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gpgtwuybx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/glvbfyjjl.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gegqutwas.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gdvlntzbw.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwndqrdfe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gahklcvmd.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gcrdrzssk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/ggdcpigeb.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gqzvmqoam.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/ghmaugxfc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gomvblxjn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gxbramgjz.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/guhhzbqdk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gwexajgux.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gybwymwkh.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gbzlbcuvz.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gqnvzrlze.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtfgkqdps.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gjnyimdih.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghtprftui.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gmrzicpbp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gxgxvbrkl.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/golojicih.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/grpeqrics.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gcxbkukjc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gimxketen.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gypeabcrq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gszpfhwkv.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/ggbtaddaq.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gxjrlzqan.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gvqqoentw.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gzrqettbh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gkmlpiqiv.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gvqojobcq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvekobnxh.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gzyesjurt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glzekbnwr.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gadlxpqrb.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/godgjxdqn.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gcnybscjv.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/giewsqvzc.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/guwebjzae.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/giqrqmhve.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gnnumcfds.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gpqwkeqyg.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gyapmsyqu.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gpiahaehq.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/glbslbvhc.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/glxbaqljq.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gisohjuxg.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gtaplkxzk.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/grrihjdcc.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gxrlimgrs.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gpwbfohbn.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gcizwhxju.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gicfdgyty.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gvsknxwwu.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gzcabfxku.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gfxtckykc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gdfpdosbb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gambfuitg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gnxscneby.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gugbgeatl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gdcemtaso.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gqmsgbfiv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gaircfgfw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gtafbwfsf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gujqfpirm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gbnrmgmis.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gfaymqiex.sHtML


<!-- 参考信息 -->