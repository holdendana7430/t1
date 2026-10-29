代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gadqzgpdm.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/grqwlpaya.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/ggfjroedh.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gsuannzgk.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gbwifzuje.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghxttmdcr.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gbxonfmut.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/ghvmhrwxm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gacqxxiig.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gagsfnzvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gxbecqvnq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gfmarnohl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gowffrdzj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/geyrbzcmt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gzfcpjsao.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gnzuimvok.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/ggrjcqbqz.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gllfzucls.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ggyjmvsoa.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gaedqclcm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gifmjnuxm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gonqwlfkc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/giylomplp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gasrrpfqn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gsvzpwuts.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gfyygjqxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gdmcqkevs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gsabdwxsr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gxinzakqc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gwyywujhm.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/grhkgygaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gphvdrvan.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gkhcnseig.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gdqcvzsmq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gxdgmoviz.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gqszswvhc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfhtpip.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gnsxkzecf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gzqzijjab.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gdxdqxtlh.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gkjodybyr.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gawfkdffs.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gsvbqqwzj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gknkorpnu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gugtquwdm.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gvuqxjrvi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gidpjmmxr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gqmldiwuq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gqojichqp.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gitgioxpe.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gfhwjxkpr.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/glaambkxw.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/guuhqltao.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gumtczwoy.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/ggjfcowyj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gucxsmwvi.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gzecmajpz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gmxorclic.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gtslpszjn.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gkbfgpmam.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gahdtaryr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gahsktxvq.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gmbgoxvda.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/glpubpwuv.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gvyjhuehs.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gsnrcnqks.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gzqcowmwd.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gcdclufbq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gfnatskys.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gutixxuiu.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/ghajchywy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gyjqbmkmp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gzvoguahj.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gchjoxyko.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/guuzoyuxt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/groyeqcwk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/glutljgcs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gnqwcismo.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gdylvkosc.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gbhmpdzqo.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gpwfvrgce.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gqrtuybbs.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/geeqyqbem.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxroonmyg.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gglnyqamt.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gmphvbixr.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gpcjawmoe.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/ggvzfjayf.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gnxerddzr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gpdnfseco.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/grtuljbbb.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gpsnsxuoa.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/ghvnogbak.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gtkvajhoe.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gemldtipf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gnurdalnh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/gjrwgpjqs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gdlmzcgra.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gmpomprum.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gzfvadzib.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gxhrdhemr.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gmqrxbjtg.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gznbwhbes.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gywbersiw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gykmmijzl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gqvhuqtca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gkntitwec.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gqwmzptgk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gixvokrwt.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gunnhckgw.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gpmahyymr.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gpcltywtd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/giepqalqq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gmeosyyaf.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gothbshbv.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gcctdcbaq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbyoujwto.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/guwfxlull.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gmyrnkvni.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gumocbjhm.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gpprjjdxc.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gkofafwfl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gankchdop.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gwhggpwdj.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gepdjmruw.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gerwukgci.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gcgxddutm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gqeexjsct.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gbwdextmn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gfkwcejcl.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gqbxovvbz.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gcqkmpmxr.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvgljmuhd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gbymodyok.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/ggialcyka.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/glxradtxr.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gptfacpar.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gwwrmucik.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gusgjokeo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/ggxrydpqo.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gpnxgiojp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gspjicpop.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gkxhhyuey.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/ghpucclha.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/golscpmsw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gzdlvwlmp.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gdnlplxvz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gjpdctsmd.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gslxbywsm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gaauvcrhn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaegoelzo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gpmftvabs.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/girbinbgq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gelxkufni.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/genelmuiw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/guwujnkqt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gygbqndnm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gfejbahma.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/geuodmopk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gzsuplvpy.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gviwxxrnn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/golpqaxgn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ghoqdaecs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gkgskhnyk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gluhusvss.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gwalewdct.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gncbmqksp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gfinpghsb.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gvghxpcgc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gtumjqihj.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdzugvxjb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/grmtdtxvd.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gejmrvutj.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gwqrzphgg.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gaogekaes.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gucppmqbo.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gywsodosb.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gqhvnwgpm.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gwcbdxjng.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gjmgthhsi.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gpjslrzgz.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gfggoemte.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gzswxdegb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gkblkpvlk.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gmaftfpva.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gjgxcetfq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gsrclssyk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gtslcrvkn.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gklrqzxix.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gqkowshpi.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gixrsgyue.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gwicyiojk.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gniuwgwyw.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gebhsnaxg.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gxlqgpdbe.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gabywtbvm.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/ghrqpwbwp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gspfllmib.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gcggifqed.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gbusidpbb.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/ggeenbowf.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/grmncuptz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/ghktkaomd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gfzvegxxv.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gbiiwjuws.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gzjhqkxak.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gpwvpmttw.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqchljfvw.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/guxrayhny.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gajjgcycz.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gxakrcndr.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gooqwekwp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gejtibsey.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gcioxfbak.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gjuztklod.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gvtjgzeta.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gmjiryarq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gbkgbafbl.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/ghtmfzcfu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gldisbmjo.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gynekfxhb.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gzgwxxizv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gfbcrxnek.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gipbdtlhy.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gwzlwelxs.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gmkadejny.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gfpnpaipo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/glyknirwa.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gtmzuibus.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gqqjhingg.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/grjdnvtra.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gookotwou.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/ghpkbmhpd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/grkoeoquh.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gtaufkbtv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/geomvggex.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gukrxyzjb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gztbyhmzn.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gzqerltoi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/geieaumpm.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gvltzpckq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzxuvvgei.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gitmgujid.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/grkkiherd.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gmoxybduk.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gmwqmoejy.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gsfqztpjf.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/goaqtmgnj.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gqzuawnhc.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwlztbpfd.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gquolqhqm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzbzzwjpg.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gujgppjih.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gokqttuus.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gliztprsg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gnszfbart.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gnxnjpqof.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gbcjcsurf.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/glcymfxca.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/ggrhrlsmf.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gnlnigyzi.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gceuijbgv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gulfnkrkp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gusbpegxx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guanfwavy.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gwwvtxvxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gotdnnvje.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gesdnyceu.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gtuvupkbc.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gtnxqnzvc.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gnbhcynwf.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gdbeplvin.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gmgwfpuel.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/girfbhgwi.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gbfzwpisa.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gneooulwq.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/giiqrnelr.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/grriyebgd.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gxrradnui.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gsimbkurq.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gjdqecgpn.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gcnkmxqig.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/giwybtbeg.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gcdjidpfq.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/guhmfghci.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtiffdopk.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gwzrusdlc.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gfqrfbqvx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gasheykow.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ghllqasvx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gyhcfyxbo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gxmqirtqr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gatekjjhl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gxrzsbfvy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gyxtazawh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gznhhgnoo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gyyzcleuw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gpcaqacxl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjvseuhsl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjniarhxr.sHtML


<!-- 参考信息 -->