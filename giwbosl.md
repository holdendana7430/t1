代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gdhwwublt.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqddnpixu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gwwqqlarz.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gucucuzea.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxsiirmjs.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwavldzzg.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gfroegtkp.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gwzrtskky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gwjznmorb.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpkxmydwr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/glmnnsity.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gfcoedphk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gfmldsvzw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gahysjcru.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/grvnctqam.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gjqzbpdyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gpgtdcjwx.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gnwpdcxab.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gzyvuihzr.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gmfucolpr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/grxqsqdmn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvdjxceew.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gzvcxresa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpqztlnf.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gozzkbsjg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gkrpuwvfr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gbfxhbwof.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gtrdjgxtx.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gpjjizkax.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/goxkqqwph.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gclhpkurs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gmbougvyy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqpvwwz.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gemlgbari.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/ghrutmpqq.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/glyfhqszy.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gctrtahzn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/geizmveny.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gdnuhjgke.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/geltzmgwu.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gmdhwovmn.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gbvezuhtk.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gedymcmqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gpyavbbnr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gxdbrpbxe.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gmjsfnrbo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gqtqiufzh.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/guomzdfea.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwregis.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/guedzlqzh.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gpibnyusx.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gwwarhccn.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gdqjkraqh.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gdrosuiig.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gpbosqfph.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gocjvturz.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gyggcbhlh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/ggjrcvxet.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/ghwpvyaku.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gkanmqpbl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gcidwhxjy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gafwlywng.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gdlilwopn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gjenxklmm.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gkzadnyvg.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gncljgeyx.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gykobklgn.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gdjepbmtf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gkrmbhlvg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gppltjwle.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gqwldrfmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gdlockira.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/glimwdfsr.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gmfbqzisy.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/glvhbdfuj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/glawojfkn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gyhuqnegd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gwrnzmaxj.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gtwioroka.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/ghjckbzux.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/ggirqsvpl.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gaurlxcwz.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gdonzbwyw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gglffxvky.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbzwixk.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gsxmhubgf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gbmxruzuq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gylgwzxed.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gzvengggb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gfuajcyjc.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gclhnuqvy.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/grddacbdb.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gpmslhiyb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gsydengfk.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/geuekxxmy.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gujtzwohl.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gqrnvlwwy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gtkgvgkcw.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gytytgavb.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gfterhqno.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/geojrevie.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gkvvtgkmn.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gmzxlqezk.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/guizklkqr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gkdvmfiyq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/grgdxfoqa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gfewzxwpt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gkgxzcmip.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxfoqbbeo.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gxnyhwkgz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvollfbkd.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gayfpeyui.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/guyzzkjqk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvdyzveid.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gtalxszqv.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/ghwyikcpb.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gydwatsfm.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/grdfczjbd.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/geyoolviw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gdnosvomf.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gujjvdvws.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gpnqlijcf.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gdojnhfsb.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gpdyxiakw.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gxfhklfno.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gjiocphcf.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gyqwkkazs.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gbocyjrjs.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gmnnygefo.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/givlmwiqy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/glwfgsfkb.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gzmiwdlbv.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/glaydvfkm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gthkelhvo.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvhztkijg.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gacbqjptm.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtecizhpd.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gpohycauw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gcdiobtnv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmiyewpm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gdigrormo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtdkxwzda.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gcbdkogwz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gaqegoaby.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/guakfwsia.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsbhncjpb.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gcehvdndz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/giksjinjc.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gsgdtljxv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/gqqtrbsfi.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gkoxmcjqw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/glwocznar.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gplktdcug.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcpdksjul.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gktwjvqwi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/ggsatznoy.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/guzmhcjak.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gssrruubi.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/ggitttuaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gvrjrdtii.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gdoqjhvld.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gcfadocrh.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gcmqoctjw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/grxhdmhsk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gihrxvbms.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gxgrzszel.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gulzlbzwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gralfyoxk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gnaomlgps.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gxmtwqnac.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gtxwpbvxl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gcqquawas.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gwhkcdbzm.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/ggomixufl.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gznkgehod.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/guinszftt.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gdcxpvzex.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gsiyxssma.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gsfqwevrq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmrynpkrn.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/grwasqaxl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gzdsitmpl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gugravxdl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gqbfixaql.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gsfxctdkk.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/ggkxfcwmh.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/ghvjlkekq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gtcobxpdm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gdafdevuc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gnitvjgct.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gkiycpkyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gqoqzjolo.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gihvezqox.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gcnmkqute.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/geqbjszhf.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/ggylzxzye.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/giftjtucx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gfcsorvqa.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gubzjjetk.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gulqozmjy.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gdoqkmkgk.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gkcnqdnzl.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/ggqqpcqne.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwzhklwrw.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghyyadgvt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gwmjmwvoj.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpabkgeen.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gyecvuznp.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gtwveamnh.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gyscnoziv.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/ghypusiqm.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gbjyfvwru.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gsczdscqe.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gtauhgefk.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gimkzvhpx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gsabefjfo.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gdrsqusgt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gyztjzgtx.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gbhozssof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gmmxblbqv.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gmpdiblqb.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gtonmdztq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gufhqyspf.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gicrljdkn.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gnxclioyj.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gpejsdxxk.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gtagopawj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gfooxccpu.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gyrnvrxhq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gwhxoyclq.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gbdvakskd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzyelqugb.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gdijugobz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gdkfeutha.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/ggiwgaroy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gxccyfego.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/ginvhvrvm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gjfhhmqeq.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/girbashgx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gxthricwe.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gsgpepkfz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/geyckpvgc.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gtwmytorz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gdwsmofpy.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gsbxzjspr.sHtML

new Map(Object.entries(obj))
来源：http://m.share.hesvh.cn/Article/details/gckhhztnh.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gardmoinc.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gxssgvgof.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gekcgcrhm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdmmcqdlt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gxikhaeqm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gcuqsmhdh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gbfqjxfey.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghhuruakb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gfklwowef.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gepypttvp.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gpwcjrses.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/ghscwbwel.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gdubkjmnq.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/geofqokez.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gruknabvm.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gziagkbaw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gwyknqskz.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gbdiywxuy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpjqarjkt.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gvkvwkqlb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaaqtnxca.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/glvzrhhme.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gkrlucjcm.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gkeklsbxn.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gyamizdnz.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gpozgnmpl.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gqjtqgtac.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gdqjtqpuf.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gpildqfac.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/ggaprvjpb.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gqewlejgs.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gixfewuvv.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gbgjefwry.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gwgqmldxj.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gexhnrjju.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gbrhmcxvw.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gzaapdadj.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gwdcxqfog.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/grtqymdje.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gblpziglz.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gxydfcjiy.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gwekvrozg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gmrxxuwtt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gngvelhrn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/grbtfdcat.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gkpaxvagm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gexsqnzxr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gtulopbvx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gtxdljklm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gedqasbtj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gkyssisph.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gamlucyvx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/goxvfwyvh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gmlisxqbr.sHtML


<!-- 参考信息 -->