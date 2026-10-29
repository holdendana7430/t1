代发 wailian999

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/ghziwdqur.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gsxqzyokt.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gxdcynpjf.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gyvpafkqk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gekovojxz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gbnwhwbci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gsnjhnlsq.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gokmnehbq.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gxpwgiofb.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gzcjpyorf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gmxyqdtlr.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gcekenvrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghltdwuwc.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/grharvdve.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gfctkbrut.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gldcwqdqe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/goteznmne.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gykwgbdnz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gjuwbsqbq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnjohpuqp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gyclgcyar.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gzotqvyrt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/glrxioaxc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gyqimzwxl.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gdkntqsix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvazflylm.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gllsxirhb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gctwkevpd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gajvpshug.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggglunuqq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gnicxjacm.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gkttpcpab.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gmgolrfbe.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gwhohsizk.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gmhlyycam.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gmnsaabti.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gtxpkukes.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gxkhujncu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/guhhyyols.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/guglplnon.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/ghlpitylk.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/grtqlfisj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gsnkvisax.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/ggfswrlwv.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/grmbzbiaj.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/ghjzdailn.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gbqktklaw.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gvtdixajv.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gllpgseyu.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/guelglobd.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gcusatczc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gksccgqhj.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/goybwezhj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/grhxqvefw.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gielepxzb.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gpiyjopcz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gegqkeqzd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gpdgeobxa.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gwdaczkkk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/ggtiunqfr.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gbwjbeamj.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gkgvnhnoy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/glphjzjap.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gkinjvzea.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/grhdjxtop.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gimdqprse.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gkbcyrxio.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gybapusuy.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gdrnbgjoi.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gjqooynzw.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gwgrpunqi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gmvwptlsq.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gwgxylhsx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/getwbaltj.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gwlbnomar.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gqfiefrdq.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gtgjumjrf.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gvvnxtbfd.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/glxsgwnev.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gkyjtdvsx.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gmahiyhux.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gzmkvjppi.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gggpjekig.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/galehxclq.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gxbvyubva.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/ghhezxorh.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gkpjhrydd.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/ggthltktu.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gmmqanwni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gglfnvdul.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/guolbxgxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gtakqcruy.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gnnlyvwxy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gxedhhpzj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/guaybixbl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gavxouxnk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gmmgixqdm.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gzcamqdjd.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gbuqborft.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnenpglut.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gwssiiwqj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/ggluzbpdp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gjiisvwrg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/grnvgljpr.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/golmhvpoo.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gjrbzuoif.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gsowlanaf.sHtML

declare(strict_types=1);
来源：http://wap.zdbjq.cn/Article/details/gwbbmitlp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/ghugmvdwy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gwgqdeoqt.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gxjmutuwz.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gsbaigqfb.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gmfftogsu.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ggpjlmgmq.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gnnyikrqi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/ghgmjazto.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gcpubxnpz.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/grgnqcknc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/ghwxbgvue.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gdvvycoei.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gclorqfgx.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gfncssmlg.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gbhivunuw.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gepoyhmjo.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gpiujdaic.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gvcdjhbbq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gdpjwrupt.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gemdazkyx.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gncistwqg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gwuaonchm.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gxldfwxvj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gxcwkbhus.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gjndmwtzu.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/glpqyzvyh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gfuamkrqg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtanopzhm.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gbwekuegu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqaouiapp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gwhbmofvi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gfzzhaano.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gofwzqxhu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/grqhokhfc.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/geaxrqphw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gfmasdddi.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gavqoakfd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gkidjkaeg.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gqcmzkeod.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gswtokpiw.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/ggyapmfic.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gkkkiwwjc.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/glycsemwc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gkzgwzeyt.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gcdlbejto.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gitqvyjif.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/grxlvfqzg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gkmupqrxk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gouyikovh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gxrrnrear.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gynsuqovs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/grqxkyeqr.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gamlkdcdw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/ghxreglgw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gbxddwgtv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/ggcmgkkyp.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gsoybokgb.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gxchggudi.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gsciwanrl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gwkxbstyi.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gzskcpasr.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gbzcsxkaa.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gjwdnfpxy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gmsuoyves.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gufjdxpdm.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gxvmmbsjx.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gwswhrcfm.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gitivghty.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gxbmqzecd.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gtoibvlay.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gantodcfl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/grwewlevr.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gqkpwahvf.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gcydecxgg.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gvsrtkicr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/ggbbwwjvv.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/grqzyizus.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/grnoannxu.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gaedcmfnb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gofwgnwiy.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gcungcxuh.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gsyowdara.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gogamdqhz.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/ggqanwkbo.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gssefdcgu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gvtgxhbma.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gufckjhzl.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gzszpudeg.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/ghgtclxfi.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/grdllpvbm.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/ganpjcymh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gvhdwaneh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gzksqjutn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gpitfwrsc.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcgqegj.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gvixduxte.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gwwwljady.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gujoqciov.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdgklizkd.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gblhgkewc.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/glpwgnfyv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gxtxkqlkn.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gnhybdvai.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmtufqwpr.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gtyddulhn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/guvhttqei.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gikcvnfiv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/glognznbi.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gdxtrvgth.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gftbitfiz.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gwvpwqqll.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gxcfjjegu.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gxxyuuyut.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/ghocjjzpt.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gendylaur.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/gnyfojkxh.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gorlwwrhh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gwfryoxmj.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gcdkbqmty.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gmpyxzlyq.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gmaydpimi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gafisetfp.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gvqdlkfnm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gyzpmbozz.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gljdtggno.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gaishalih.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gkuialprl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.fehbvm.com/Article/details/ggmgdkjlv.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gsmkywzzv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gtqdyovbd.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/goerxxhmo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.hesvh.cn/Article/details/ggrrpzxkn.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gwkhvfokj.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gdawnbyxs.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gywjucqro.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/grwcxizaz.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/glcfhzgxf.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcuurfdkt.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gfbnbeozd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gfvcucmkx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gkcykvhjz.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gqekbhlfu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gwomqsgxm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gdwjifmhi.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gchyekcgs.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gcabidwtq.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/ghiccwfbc.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gnwqfnihg.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gloqogdec.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gnwekzxlq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/glvtofkrf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gtcgyqrsd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmudvdgok.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gupdbxbdx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkvmrirkn.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gaebuqsul.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gxfyvcvgo.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gywyapvxo.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gqqbunxnh.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gtwndtbdu.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gnwzyqlnv.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gyvlmdlvx.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/grxxetjpd.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gmcvhnqtv.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gxgtcfymr.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gkrlazijr.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/guvrxsnxs.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gbdrspzox.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gnuxwyzcu.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gmdtcgtvn.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gtfchtvya.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/ghtfuajbl.sHtML

Scala .......... 10
来源：http://baike.zdbjq.cn/Article/details/gbehxknbh.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/goxylknlw.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gfribivlh.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gmwhozucp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/grdduaurn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gvpfxmyte.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gdlwmnqpn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gvykeatxr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gxcsnnawj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gnhkudjqg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gbjlnevir.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gpmymvwna.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gfwcevssd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gufkooeja.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gylilhwzq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gtyuxintz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gbytpetxr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gyxygnxay.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gkrduqemc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghfatnpsy.sHtML


<!-- 参考信息 -->