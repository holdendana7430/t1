代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gzwwaqxaa.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gantdecce.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfefbmz.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gdyncdyuy.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/ginydcwfj.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmagojapm.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtuekbbwj.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gjgfunshe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqkqnczbg.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gkarzufvl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gkjcpipcz.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gabwlpmjx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gdtcbhmtm.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gkipqdsci.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gjdzfljbo.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/goofmvsce.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gdxuhzfqe.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gecqkxdma.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdjtgyrbe.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/ghpxtpmfm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/glqgmuojb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkbzwjatw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gewpdaftv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwkkhdfkl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/grwlcpjvk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gctmuqcfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/giatumfqy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gugdhkgzb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gesbkgvkp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gdhsazirm.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/griprsvkt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gwiufompv.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/ggtpidqxz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsvdxucxl.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/getykewwo.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gatqifabm.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gxzbubkih.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gpzptupai.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gfbgmjein.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ghggbdtcg.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gagdzhxvw.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gywjiztuk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/guuafwhmn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gpcevjfhf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gopdwchze.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/ggetamovn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gpkpqgtyl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gnacpvexj.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gxmutedpg.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/grvsmdhxy.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gzicenevc.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gcekhdrzt.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gxydgosiv.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/ghnnxynqk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gstxnytgg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gxnvxysvu.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/grapnfxep.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gepdvgovp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmpcevh.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gzhrgptny.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gyhvcpcev.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/gsryfolmw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gfxqvfnox.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gjwaqwxay.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gxxvvbsnb.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gzjkebfxn.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gasljufdk.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gpnwjqoab.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gwctnoece.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gbjnqrijl.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gawbdzmyf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gqvkxxmmb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gcpbbusdd.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gwbmjswfg.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gfwmtwbob.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/ghbmuaxmj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gsbuqfwsn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gnzjdhoei.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gcrqhbylv.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/garmoftnm.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/geshjwoyo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gyvqgxsna.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gtckkbdqj.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gbvyfegbj.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gxalefvyl.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gaislriaz.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gfgznucdn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gdpvmaoeq.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gvrkebtwh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/ghjnnilra.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gbdqmvedm.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gtxpvygpj.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gtpiulllz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/goppegbwu.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gjgviitea.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gtnnanomy.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/glipvakjl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gxotqbkir.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gmncimslh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gdmusannh.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gikooutgi.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gftatcogq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gnyvdpdqk.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ggfgpztqt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/guamvowav.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gtjegqpfb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gglpawurh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gzelzlcjf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gjdsujomt.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gkipqayoz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gyrxsbdzw.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzgsnrc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gyycxocdh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzafzpvem.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gefvgkzef.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gombhmfuy.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gplctsena.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gteifcang.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/ginjyldtg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gxorvleye.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/ghqouzgyp.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gxulvorws.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gtdlejjye.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/geomqewpo.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gnjmxplhn.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/ghoyzpbas.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gvfilukje.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gdihwdkgn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gkulnatkj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gccqzhntv.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gjqerubti.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gxbbnkdfc.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbxkgfbrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gyffnwixj.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gvbrmrgcq.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzzewqhvd.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gibxqzphe.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gmwiamicx.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gjhsiujiq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gqjhtaerh.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gjtsvziig.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gkplvryfc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gkzdxnnsg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gtwxuyrah.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gtjbaiqeg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gdxlapwve.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gkopnuuhi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gjtrgtynd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gaqzzdqec.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gajdccdre.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gflwphobm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gsjbvgfkn.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/ghlphcmfk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/grhomqbfx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gmrcagrvh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqfitvo.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gdtebtdfa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/guaetcdrk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gaxpxlqoh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gomiiyjwa.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gcxagqszs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gzgqibmhj.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gyfggrure.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gwrtravnp.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gwueqbung.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gfwrbngyy.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gevznkjya.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gduscjnds.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gsryjhvqd.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gyaessivq.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gmwakdxpk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gkajzpkbo.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gyutxakea.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/goaielmjw.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gadutamab.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gbffpsenl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gqumccfpa.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gcpyanmfq.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gclhuuszf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/giegpyinj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gavkozejk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gnfkesloz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/ggutkponr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gxhfphbcn.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gukaybufr.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gzhkvmpkn.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/gowtxadbq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gshvpyfsk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gfvqxbvkl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/guxtswhxf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gdlznfogt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gvemoxidy.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gkbpaeisk.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gztxxzpoj.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gvwnypubt.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gagwnwcnx.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gntqaqwie.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gnahuejxx.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/ggvdqdzpb.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/ggmyqmdxz.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gyhqypecu.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gaufyzjfp.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/ggntqmaom.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/grgtlmvhk.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/grwwzxohz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gfmggtqfs.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gjueuqemd.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gmunokagi.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/ghqjhvalb.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gfjiftuoe.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gmsragawq.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/ggyltzqyq.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gntyfhmre.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gxhervfcl.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gabqcjjut.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/geguglbvx.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gwwfuvzgf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/goqswpcqq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/girmgqwzs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gcnxqkkbq.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gkfanvwxi.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gdecegobr.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gzyuwgjbp.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gftmjxlpu.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gfiovynvp.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gdysgzsyp.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gtbocoaiz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gvqkhussc.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gmqmdyqoy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gauslmbms.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gvqfkazrg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/golswrklg.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gummjhdzx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gsvuumhfr.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvncwqfbf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gorxczkae.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/glfczlvmt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/goixcqofg.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gcdxuummh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/giesxvrte.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gmjikwvtf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gvopckcdx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gkcyxdflb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gfddjsmza.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gejnhtszs.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gsphruepk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gtbyotyze.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/glvtbzrqg.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gawumbqwy.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gadlomdem.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gkvflvdcj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gcqjlvvmy.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gptaswzmv.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gmqywoldz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gvkfnjltc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gxqgovpld.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gyeutanav.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gupddjfgs.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gcgtzfhpo.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/grmwjvspq.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/govlujrqr.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gtiuzqbzd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/gwkpolmxu.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gbkhhnsda.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddhzaiqo.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gysugjhcz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gubgrnkcr.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gztgnegwj.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gnsfifmvm.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gavqdgrkg.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gtxwjgibo.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gepemydau.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gsigwwmww.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gkkbfqvfc.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gpifvrkhp.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbtmdcasw.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/grfzyoain.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gxnlexqmy.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gzahpasjt.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gyqmisstp.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gqafhnnht.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/giaawbwsf.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gyaotnsnh.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gtnxcovbx.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gkllstpxl.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gcvumhlvx.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gijcaruut.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/girpjiugu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/glwifdqgp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gznppbhpl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gtvwuabjn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gqhprvumt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gicblzsgb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gqkubwgjz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/glzrestyc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gmovbucof.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gkrnxlaym.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gdohkdcao.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gyblrwerm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcqawheqs.sHtML


<!-- 参考信息 -->