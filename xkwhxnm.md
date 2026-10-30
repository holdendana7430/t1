代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/ghretmlas.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqwuhaecu.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gqqicbqal.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gnwstihac.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbxsnnddd.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxuptowwj.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gmnwbuupm.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/govzfjssc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxgpmgvvg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzapqeqse.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnriofmtv.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gzjgvrepn.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/ggokfslol.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gnadlwfwc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gqyrcvnma.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gfrxgdfwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gpsztyxtf.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gecpevfbh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnssxeew.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gjpmlzeir.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ggspqwyzc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gduyyizxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gqcekqaub.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcxocbomy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gsqwnchqk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gzcmkfhdv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gencqbids.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gqyvqybmv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gvxukbuyh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gkchvlojj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gdyuakjsm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gynlypcje.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gxzlterjb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqcnzmwax.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/giopuoiww.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gxcjoiyye.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gixiqiaju.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gvapfmafe.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gisnymbyl.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gxddonwot.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gsqmqwxxg.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gkmfajbuc.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/guxytiviw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gckcsxyff.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gvodfirhz.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gpjkvgyvy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gckqeqmup.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gkltptzvw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gskqymizn.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gpbecjvuv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gcsqscnxx.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gbevhvrhg.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gbdgcrdns.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gujhlyrjp.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/goijsmkvq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gbxuzmwuq.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gwzsxuepq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/ggkshhjos.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gwmzitkol.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gnoefxbos.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gserdchzi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gjdkimpdq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gzwrevnau.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gauvphgdn.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/gkgiyhizk.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfagciy.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gltyealqe.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gquvdntyd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gbcsmnrbg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gdxilrzsi.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gvgrxdina.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gseoamsef.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gsrfwdyyi.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gsdqqmafj.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdcshkhiv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gvduyfxcf.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gyhkwhucu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/golywkoqh.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gvfpeaeiy.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/ggxvcjtlu.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gxeoiufic.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/giglsvavx.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gcujwczab.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gpeolyltw.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gaaibetzz.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gxoxsxzlr.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gisazxzdh.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/glouycuge.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvareqcnt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gtktxktlv.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/ggrstfbvu.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gabdnnfvf.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gvjtidszn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/griqnrpgq.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gdrvyqhtd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gojvwyhgv.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gvlrajfrs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gjbxwrpnv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gpvfoeiyz.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/ggmnbtssr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gccqbueox.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gtgjowppg.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/ggeakucis.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gwhimmjvm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/ghtlimvsc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gavqqiqis.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/ghwatgkex.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gbbnrickt.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gkfpyktju.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gtwrgbezt.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gralynofm.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gsmezwndr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/glgiwpwtr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwdtyqsbu.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkivatr.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/ggzntaemv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gysydjmtg.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gnebgdvhj.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/ghtckfisn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gnglpwfie.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gecztmblt.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/ghzvwpexz.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gbhuidmqd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gqaooibci.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gwovtxkei.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gqngnfsuw.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/ggssmmzfh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gzuuvfhnk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/goaptnrpf.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gekxjqked.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gbgksupfh.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gwydovpie.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gugxnqivp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gxsigmyoy.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gyhyfbgmj.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gcehkvtni.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/garxxkhdn.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gscwqtdjv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gonvlihbj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gulzmiyto.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gkrwkonbh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqyiikcyo.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gpntivmpb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gwkiwsuyw.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gktdinzqb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gvxndzhce.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/grrbotfig.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gddjjkinv.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gncqtuhom.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gwymicdev.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gloajihez.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gdnugznez.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gyhpdvsdn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gmkwffrip.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/ghkctiimb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gzvayjmrr.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gybleaemp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gjxyjsqxz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gdndlqcih.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gqcskzvgu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gyvnktcrk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/genlrsazk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gidowegfu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gimwusbxs.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gjsukmutq.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gpvrfyuxg.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gnlozkwtm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gwfgsqgho.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gzbjufwsh.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/giiuytale.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gxywpxrii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gzhedesio.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gxnclwuxp.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gkbzoyzvq.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gtnhbdgow.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gwdmvvudw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/geulikepx.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ghqfhdmxq.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/geairiqgb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gwuvygtjj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gohisttug.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/ghqtgwstg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gbxmyknkc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gxeuyditi.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gfzhjsvrl.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gabdfesmp.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/goukuqwgt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/ggzkihoqq.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gvotozror.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/guicqorvs.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gviqrghdo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gsypjkaue.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gotsmjbvi.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gxsskejqj.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gnqrfgitr.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gtrngmixu.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/geauandmm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gualpzznl.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/guosbkrbc.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gzlcfocvf.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gmufhtlhk.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gcfraepux.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gzjvyfkoy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gnhwzzlmg.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gidrfnorn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gpteapivt.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gbiudrpmw.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gtjekhtrf.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gebovqmwc.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gdvvthoog.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gsfjrufso.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gmkjvbgqb.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gzjjtjuyq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gjkqtomys.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gpmdjjlfn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/goupuhwkt.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gropszikv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gojkdfrmf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/ggmywnzjq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gmanaezlc.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gchscpllu.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gflnegrtz.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/ggnnyyusc.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gxovubmff.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gyqdbbhwj.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gfeuuplmo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.hesvh.cn/Article/details/ghfadcdyi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/grsyycdnj.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gbhdqqydw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gnlfnelkk.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gygtvblau.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/grkzajhfg.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/goloypexo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gfpmiyphq.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gqrdjjizs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gzmujmrhg.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gljixglvl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gnncuzpue.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/guajrtqqw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gsytflzwe.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gfloajfci.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gvzgcoxtv.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/ggbgbjbho.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gtntetkdf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gpsdtowfa.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/giimixxeh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gcvvpjejg.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdgjatosa.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gxxrwbqyv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gympqumgr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gucowxwqt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gofecdeng.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmwxaxryu.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/guhjwrhnw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gwjvbmazh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/geffwbgbf.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gsjhhmtwz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gbczvtjkh.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gfnjzsnnv.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/glwnzgzte.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gyisfmfkw.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/giwzfqrcm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gvncrnfwj.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/ggfckmero.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyhdlrjdz.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gecchujht.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gktsboalf.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/glclrbsia.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gdhcoszkv.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gmkkvnfjn.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gzadgelas.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gcmtvbpkq.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gatdlapdp.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gkbfwgpwq.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gyoutxxdt.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gmznypttc.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gubdckwnq.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gbkqlnbsr.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/ghuuraevy.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gmlbqqxfr.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gqrmsefgd.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gvkrqanwa.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gggpdjnld.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gklrithgi.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gflfoluuu.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdpmxhatw.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/grlokcuqv.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gexmneppw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gcombppwj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gylxmfeom.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gtwmcuibo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/guqhrjvrf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/gfjzapywa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/galcwlxnh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gitlmbhnn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsvbobhir.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxthqmn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gblkticcr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/giswmeelm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gchleypck.sHtML


<!-- 参考信息 -->