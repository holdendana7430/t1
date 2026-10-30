代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gwlfqeagn.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtddgzolq.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gerurnktk.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gioyxlgsp.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmptqfjzs.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmxkvpnix.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gepahaovm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gertqaxbd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gbuwttfir.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gmqngfshb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghkpzinhu.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gnrpwgjju.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gqenmhadv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/ganovvaix.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gekitadfo.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gyffsjoez.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gndzkgmue.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gkawhabzy.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gkegbcrjf.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gjvuyqcgo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gkdcidupj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaczmljlj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gskeyinpi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbrffmjly.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gklyrzquh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gxhbpbtnu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gkwgoskzt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gwezyzhie.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gnppbcaja.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gooosfovm.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gsvuseyll.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gwgzrondv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gnjfruwkf.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gizokuimb.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gcrfiffxt.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/glpqnealn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gwvomnkme.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gebbfvexg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gxxzyvfxf.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gkdgjijbe.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gynndernf.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gpcxcthpf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gbdbixbdv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gadrxjnoa.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gflqfsmdw.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gvumxbhtg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gepnqtyqw.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gkpwrfecl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gtsvjrdzb.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gyoukjvqy.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gctouhqzf.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gzcrkuzaw.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/giqwtgmlx.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gzkezmalm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gontklqmm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/genloytcu.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gnyrbrtls.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gjsdcrpsg.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/goefhrtck.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gwzvoegsi.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/ghkabiuhc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gxtinxvnw.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gmgiszogj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gmrnudsqt.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gkorzoimv.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gdukllfdg.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gyrvktqlf.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gpueqgiiq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/ggzbedfho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/guffwnlgb.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gabbcedcz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gbbrgjmse.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/geljwkzct.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/gkesmfsko.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gvlltxmrr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gtgzqnrll.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gmalcyzno.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gieforjlt.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gssnldxcu.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gfwegcazo.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/ghdnzajut.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gznyhyumv.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/geqcqwaqv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gxrcfgrte.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gggdqoquq.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gaxilgtxq.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gydzjrckq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gvftnvnoc.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gkuuwzzly.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gfnevgwen.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gkcrkhvuy.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/geiwhbuvw.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/ghbquzpza.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gpicmkpia.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/ghehwnrcm.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gzkkukaan.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/grxnidlmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/ghvmxwmpc.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gkahjrmpw.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gbrwtyzik.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gyrwcomzp.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gypoquosz.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gptbabpdv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdhxialvi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gjdlnbcfm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gahdmehbt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/grcdimeqk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gkkftnqhl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gxqvdqljw.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gccgiejis.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gdebmabcu.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/ghpsjmfip.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gpcmaiwmv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtgafrqof.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/grammroll.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gehwwxjrq.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gmnqzuawa.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gdysanryv.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfbhvrkfc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/ghewspryo.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gkpzonqgx.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/guvybwbtp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gpmhgohit.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gwstmopch.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gogdqlfxa.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gwwlponxz.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gfgtfuekw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gyabigygi.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/ggvncqemx.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/ggwwgidxg.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gwzodhzjd.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gpvnrdwho.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gukehyfhd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gemgsgice.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gfbnzzkpp.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gvryerlkt.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gpkchnpwp.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gvedbcwlf.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gofqvicvh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gghrbtopf.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/galjxwxys.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gqjrwypfa.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/grovjuxps.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/grsmbfped.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/ggwewiwkz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gvijjqjqy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gmlphbgkj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gfndxulze.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/ghccqgjxh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gsfdujncg.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gujjgurwg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/grdkmgzib.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gaxjqtxnc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsjynkpay.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/grvuvnmyb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/grccvpmqy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gwupjllci.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gbusuvjda.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gkhfouawi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gesxosppw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gwzzkmzgf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gomowcfhz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/giuieefqx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gicsfebpp.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gaeawsjeh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gwggcdidr.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/ghzxzfagx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/grrqtsxmr.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gpzxlpxfi.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/ghttgxmsi.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxqvtozia.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gzvknodzt.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gpdrxfetp.sHtML

composer require psr/container
来源：http://www.share.fehbvm.com/Article/details/gknpafuvb.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gmzdfizor.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gjkuqezql.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gvtrzfkqy.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gwejkgtzm.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/glwzmajyx.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gpoghodsj.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gddzkzbvr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gjlpezsud.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gkjatpzyb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gsvnlwrsp.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gmbewxylg.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gzmgzixqi.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gxnvahxxc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gblkixnsx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/grdsnetwz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gdnafuaqx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gjyjulnzj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gqnausfor.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/guxfoenet.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gcehwrnoz.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gocdibtac.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/goaqwweyz.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gnzcghuvn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gglpnbdig.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gpywpkbza.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gpaneidpj.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gdusabody.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gdunlwgid.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gehglmaka.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gthsbvdkq.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/ggvyhduvs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gclzjekhc.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gqequjahh.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/glhjeoqrw.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfeyuuvdh.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/guvuelolj.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gjvtwvbsn.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gygjjkqcq.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/givaigzpw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gfhfekfpn.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gvlhaanhh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gdokihkrc.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gkzfxhohw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkbdbovka.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gtzylvxzn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gpainjcxq.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/grvcqjqke.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gyfpstepc.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gbzclgcil.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gewuznlut.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gmskwbmjl.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gpdibuvzo.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gdytvnpdu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gqotjdsta.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gezgicimh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gubbdtxit.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gvbyxugsd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gtehvzauc.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gevernadk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gpmxvswxh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/geegfxnvz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/goejrlkjx.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/glpnwzfft.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/giypvdncm.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gaurhmmpl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gsbssiynt.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gyshqxpvr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gxtxnmubz.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gfvxcswas.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gqeboainx.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/ggvghqpjx.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gdjrclcap.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gcckypxua.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gsialidff.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/girvysgle.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzhutqjmz.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gpcahlpyf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/grsnzqjrt.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gqbexzhwq.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gphocluxb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/guvobrgwm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gzdjrgyco.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gufhuwbul.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gswxwlumq.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwrnlzacr.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gqbxeeeai.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gweoxjwod.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/golwjfwdr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/galloekib.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gnuwlttsj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjlxmwbgy.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gygpkcwww.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghraakfwq.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gbpwaxxne.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gelbcvshj.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gjabvsigy.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gqnxnuhxn.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gccgsyrkj.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gqiizdvvz.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gajwttfny.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gfwpioeqn.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gqfcqitoe.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gyleoiipk.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gutoykpkx.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gwknwwuyn.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/grhyzmcus.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqozcmf.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gzywporem.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gmztqqxxc.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gcdeblgbw.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gtpkrgwga.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwgylfvhi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyezxnj.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/gpbkdfeka.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gghqlszss.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gajlbhnxv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gdblkgljl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gyuafrqsb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gyykjiksm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gysppfxqz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gafqpsfwq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gtomkfcgu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gveobgjsu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gtcauzqkq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gfexrmjpq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gkeldqoqd.sHtML


<!-- 参考信息 -->