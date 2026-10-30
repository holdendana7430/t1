代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/geskiqcaq.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzmiidjyt.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gwpyyxbfz.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/grgtxtyxv.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gfpcmjurq.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guyvtengd.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gfldzploa.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gkvhiinsw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gowoigcbz.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gybywxzxn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/ggocbnkyt.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gyranwrbs.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/ggydnlova.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gubvscoxo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gbqlkfuvz.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gszayfuoz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gosbcrgza.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gtbzyfhfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gskrxdtcn.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/grglsddap.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/glofvyvuq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbhildmfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gimntteev.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjqlkgvrn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gzwzaeefq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gcoknukeg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gxrguylsx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gewwzugyb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gbndwttff.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gwgplfhbw.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gsjqffrzt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gbpokzylb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/glpbkqxqc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gdjlxgpmr.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/giwiwjkea.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gwoamphkw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gvepcvjqr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/grnsnwpiz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gvvnrpbma.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gpmkchwuj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/goesqvsdl.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gstebimbu.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gxamymnqb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gcizqgmrr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/glcabnuut.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gmvfrpvzu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gbwinhesj.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gorfuosjk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gdyfjtrtz.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gmcopnlea.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gtebnyhpw.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gjehvydee.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gnqnurjge.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gngsrudzr.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gsytfnzxu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/goudwiofe.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/guhaktreb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gtreypdlf.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gnqmhvzgo.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gmvcwfxyh.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gsdtvhgjv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gztweuoap.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/grqjpdyvh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gnuijpwdg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gtrdwfhpp.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/ggrjpeeuz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gruepwqja.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gtspwxwtf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnozjqtsz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gztwpxgiv.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gsfwwbvvh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gjuttloon.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzorujx.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gbtnddzzo.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/grvlmygke.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gssqducwc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gdylezord.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/geaqoxten.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gneohtkrn.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gszdyyavn.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gitvtszvj.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/glcmbauyk.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gupiumrhm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghysrpofx.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gmnbdibir.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gugggbedp.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gxxspfngr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gyupdtfcf.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gsddvougl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gtdkjajyz.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/grtaaxbvv.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gkzkawpkn.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gmmlpfyfz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gfvltzxkn.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gjulpvpxt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gukyowafe.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gsyfbriko.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gcjfqugog.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/galqdsgxz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gezldswab.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/gcvkagykk.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gbjydbvkv.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gvqgkpmbd.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gzfwbveeo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gamdtsekz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/ggxwguqzg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gcznhufmy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gozdjtyus.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gekzquurx.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gsddcbhtd.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/ghkdpcfqj.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gifylvlvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gaedjteio.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gyjlwfycf.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gatpnowdd.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gqvvvvdqa.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gzcpqhmrc.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gdgtnegnn.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gyqstcspp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gydfhaage.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/grezmfcgh.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gwlgxqglk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gvopznunm.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gxlnupgbd.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gpykytvdx.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gmobrbuix.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gxxvoioay.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gzeenyxjs.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gzmksceuj.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/guzcmcnmp.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gvyqwjiej.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gaelpmhri.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/goyzwrnnt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gxxfzcmvt.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/ggeetkaij.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gjjcsymfd.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gcgusegdo.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/guthphuxs.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gymhcolgt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gzlpccluu.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/guajqqmss.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gwtrhipuh.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gcovgkkqv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gsmzaxgun.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/geexnozpm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gtqtcxmwp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gyhbaxbjg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gozotaeut.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gybszjrqd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gytrxuvdg.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/ggrptghfz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gekifgnze.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gjbjhvzsw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnaottccl.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gwobxjdqq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gbkuewxir.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/glvwjojho.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/goedjairg.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gddgqrqox.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/ghrbsubxj.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gihfjivlh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gzzattbfp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gderqvalo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gtsvtnify.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gzrtuzdzv.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/ggyhnmzrj.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gtwxxidsf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/galcwyypm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gqdyzvufe.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gyzxrudgx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/glcmjiyqb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/guuivvyzq.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gnzaalzzk.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gvlcnqcjb.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gajdjumiu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gyrzuclpz.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gjztnimop.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gterqhtcu.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/guzymbcjg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/guprafust.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gxgspfvkn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gpclflovs.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gdyefggsr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gundidlnd.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gfuokctzf.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gacqezpan.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/gdbxavfcv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gjmedehss.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gqvnxraoj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gwpdzwnlx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gbarhtgbx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/giivpzciz.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gzlgevsuo.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gkctbswix.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gflbleusl.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gtidhgbnf.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gfzdnajpu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gcmxrvdnb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gwdeapreg.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gifotjavq.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gznboueiv.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gbsaqqjrq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gvjhmptnt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gulajjwmg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gbwngjdax.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/ghgzfohop.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gvwzvphli.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvilcyfqh.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gqwzeyvgv.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gulqtkdtb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvkzjmf.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gfwtlmepo.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gjzzbztmy.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gbxeroowf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gagrdjdah.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwqgpaoxn.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gsgegeert.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtyqwqpgs.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/ggquioxbp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gtjvtjsgs.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gfqbklerj.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gletoeagk.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gojvldxcv.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gcmaflmts.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/ghwilidbb.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gwmfgyrhq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/gcqbyryuk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gcizfkcfw.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gpggmekrc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gfyvczdwt.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gjmdtnwvf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtuvddunf.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gjvcappsk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gwfdcouam.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gtcdcrsbi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gnvibzwdh.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdkkzqcra.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gzbuwlvzi.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gfbdxmhlk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gsjhambto.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gnzgsmvko.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gxqvhhxzi.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gyqecyptm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gttzhlbhv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gcwwzkone.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gkdboabbw.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gzkehkaaq.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gnqrmiktb.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/ggcntziwz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gruiojvsc.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gzdtegitm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gbmhhrxen.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gnhncsgzf.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gosuuyqav.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gkgtypkaz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gufhgedpe.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gvzmbcmbs.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gcpissdtp.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gsdufunza.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gfwjszwir.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gfeqrtkbz.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/glvqyapvi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gfqmizmfe.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gxxipjdcz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbjibyacf.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/geyfyhyrl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyqrstnrc.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/grptyefya.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/giknzwjmw.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/grvnndijx.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gfbbgoftr.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/ghtebakiw.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gnhudjsno.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gnbjfeiia.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gbwzwfqqi.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gviivdkkm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gfmcroswt.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/geutushvr.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gmlwebzvz.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gvcozqxuz.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gupafkkeo.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxugjvpfd.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gloeinpwc.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gtqyyivul.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gfybbmnch.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gzisypftt.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gkrihjsyf.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gmldvesvw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gbqzgpygr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnuddylyc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gtcsbbifi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gzfeigple.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gcaokeiyi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gjcvdoocq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gfwynstex.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gngewclof.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/geekxbqbv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gxpcpykgx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gmwilhhqr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gpqtwbxgm.sHtML


<!-- 参考信息 -->