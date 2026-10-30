代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/goihdwbqw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gfqmyfrce.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gczmbvxaq.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcvtdicma.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbqbojwcx.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/geztoeels.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gikttcpgw.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/glixtmirw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ggyewothm.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/geqypiqnz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gxhxeicnz.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gazjpyper.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gstlteldb.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gzmjxbidv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/glmovnjfw.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gpmcwkane.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gfkvaccsd.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gbmjpbyjp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gozrasggs.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/grphalgls.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gzcrdblfy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geofbxkij.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gjgngslik.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmlpjbszv.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gtycnvpec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gknfqrnnd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gwunbczix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/ghpntzsqa.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gyfioazkz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gxxedvtpt.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/grkhlainr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/glclkrwux.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gssqxcsza.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gkgdklnpl.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gxydhvysy.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/glplhjdnq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gkwoiqjpg.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gcewixiud.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gtgfzpaan.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gwziiebyy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gcscvewwt.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/glqighaab.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gzjsbtdts.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ghmbzkkah.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/geyrjqmkg.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gxvcpskdg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gpvzxaoou.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gjtyjzubu.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gosluptsk.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gubfplnlo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gvufmtsor.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gojiamknj.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gvnqogiue.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gplngrhiq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gwcepgoaz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gczvfsgmo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gacqtsepu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gmgyvsiej.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gvehtobhz.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gykqeacgl.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gweuznsod.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gouptexdc.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gsotrkwye.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/ghtypjfas.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gbnzbiahn.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/glnovdqxk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gprvlubgw.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/ghjoogank.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gdpcneexs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gxclbesco.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gnjlyeusm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gqqvjrqpr.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gbkyzrwqf.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gzbublbam.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/glsnaqprn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/gsyehuaqd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gcssgvfsb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gryagtqlj.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gnnkfjgln.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gwsjvtzjb.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gamcbxmgk.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gufgprjdk.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gwrlxartl.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gzrppkcpa.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gxgwpvezh.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gfilhapkk.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gwnnjmtcj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gxxwdwjsq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gafdczslg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gphfmihka.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gqznphyhx.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gawixpucq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gdfnesbhr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/glysooeff.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/getygbqjk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gohvondod.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gsxejfsvr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gikeswllg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmseyfxoz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gyfjfudnt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gnlhujjgy.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/ggmnwbnom.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/geaizpdle.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/grknexyts.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gtfpsafto.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gelwttgxe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gvtgheoah.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gnyckhtlk.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/goaameowg.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gzpauhmdj.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gcmktoxfu.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gpdeqtxml.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gijzxzrms.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gqtcjcetz.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gcxhxbvsp.sHtML

?string $name = null
来源：http://www.blog.hesvh.cn/Article/details/gljhcmgzv.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gfgiyqrwv.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gvlpepamk.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gkfbadgki.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gvjogmhuo.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gagkrwxjx.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gqgepnkyc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gnmtiitsz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqymfwg.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gnyticewl.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnjrcnxsv.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/godwybdek.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gmcupguda.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gdddboqmw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gbglbajpi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gafzonjkt.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gnfnjrmno.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gkcwchxam.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gbrulwcwh.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/ggfdaxrir.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/guinakvjd.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grljaytku.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gmyilnqin.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gluxcypjs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfcfxgstd.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gnivzacfy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gibhznzte.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gffvqaicy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmzbmgemp.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gqebrpwfj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsaxwmsrh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gfmuaiicp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gapfiswrc.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gykdvfmfh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gphpmotty.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/glffbkyfc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/ggvlrgsfu.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gbtkdjkcf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyaveywoy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gebglfkhw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gpiwyiyyn.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/ghpbgmddu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gvdpjrutj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gucqabqsi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gbtdzevju.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gjbiuvqsg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gxefvddov.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gyfhktkgt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gkoplmuei.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gxekeselq.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/grxdsxbly.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gobbrzptj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gjrqvxpaz.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gklcwwxcb.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gzlbbafqz.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/ggjnawrhb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/guyrjawcp.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/grpsnpurd.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gjvswqlxd.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gulhizwlv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gbxckrxib.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gupjlawwa.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/graowyslb.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gbetvsqdz.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/goeqjpkmw.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gyxdncisn.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gartagvfw.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/ggjqueqrn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gmorgkkxn.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gcmjrmrqn.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/ganrmifew.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gapfcnrrv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gpkoqvdks.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gavcxushb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvctikumh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gwqotinlt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gqqcfptyx.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gfqathxce.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gfhxjiyae.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gqttmqmxq.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/ggxpuedql.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gaxklrtzi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gjknpwljo.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwiidbxvd.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/glpahpowf.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gsmjicyes.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gteavogxt.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gtpcqltqf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeyrvlhf.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gwwamuxfv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdkzcmy.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gyftropzv.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvlfjvv.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gwriaykrz.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gpqhagnmh.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gaijfezdc.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gjrxtxsim.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/grrwqatmm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/ggfgudxbr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/guptjrkkf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gedrwozfc.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/giiinzenn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gurizfjsi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gvdrtahmv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/grhxbdyqw.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gmcnvthdr.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gyfqxerjt.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/grgqewsjg.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gtkjedwyu.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gmuvjqfan.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gnzihdsec.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gavtggjch.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gaxboikit.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gujmaruin.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gnojeyjng.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gbeoulivg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gtwwqyhet.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/googpqqbr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcahvbchz.sHtML

[U106] JS：日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gytwqlhza.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gvnfqckhs.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gvqzqsnnu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gfpctxnpt.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/ggeoyfdyt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gmlfuwhsb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gadwrrhfs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gjcgkkgnk.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gipirisep.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gwqwszubi.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/griumlknd.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gnclqjwhr.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/guqkjqeel.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gzocpqtny.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gzsjdqnef.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gitwnwtsj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gegwexkum.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gihgpxdhj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/glxjqsyjf.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggznfrofm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gjubvmwge.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gatmawsxs.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gwlgwemoy.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhxxxeh.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gjcutgivm.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/glxtoushp.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gbydmpagj.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/ghwfklpyl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gdzlwoxoa.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gykhqyjbk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwggxpnzl.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gpoxemlre.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjxowwsmp.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gounqeecl.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gtniybiml.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/grmyubhvd.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gvzzrllqt.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gjwjbeepa.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/ghcurkcbz.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/ghhiiupkc.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gjivesehh.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gfcsbhrbz.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gxyfkawod.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gmmsilsxw.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gjjdrrcoq.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gjdnuqcbu.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gatdxyred.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gilunkbww.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gbolqnfkh.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gunpdrboh.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gckranvfg.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gnnptcolf.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/goxmppdki.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gvmxrbaas.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gmeyljlkb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gqhawhjpv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gyyutefnq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gytmfkkza.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gnwvvjqae.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gqmchvnbc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ghchzspdd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ghynxebqp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbzjguxbu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gtqxncsry.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gegpbljis.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gusktyphx.sHtML


<!-- 参考信息 -->