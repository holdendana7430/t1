代发 wailian999

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gejbjfmix.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbjbcxufo.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gihqnhwqr.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gkmwoadmv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsdhgznyc.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gzheyqclm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvipezsqo.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gcfslhawj.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/grsylijbo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gnowmzvxp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gazamjeys.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gnqymkqql.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gthtbkoom.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gjmyrmpya.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gnlncbxzy.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gmnezqxdc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gcecgjxkh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gulvjsluf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gorcyapbl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghrfmtnfl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gaaeyoexi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gbbubuuae.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gamwagfpl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gduiuhhqw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gononjwmn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/glujsomla.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gegsqynpl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gjxgfjvgw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gsiliomiz.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvnuswpyn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gctwgxfyu.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gblldwsjs.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/glptaigpr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gxtdzdbkk.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/ggswtwxkk.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gmpgahkcj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gtfgwoywt.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gppycnmvz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gxqlmqvop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gskefxdje.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gxnhgizsc.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gzdzkxbqt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gcqtglmkp.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghccvoawb.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/giiayeyqo.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gbdixzser.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gkhozckun.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gkjeeihix.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gjgvkglpm.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gwovitsdw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfbpvyn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gzxcyozkb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gdbgmvlzd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gslgvvqtt.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gxmckownn.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/goerwclpx.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gfjvzsovc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/ghxxypsgp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gelyazbct.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gbdgthiyf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gegjccyzf.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/grzhcaysr.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gunaqioum.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gtbibjqqe.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gqjentrlc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gnygyoxvo.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gihwnaaek.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gpzowsujj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gseqkhzzp.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gnbzkexmh.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gzolqilvn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/glestmtrv.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gdbvsxwwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gncyumuho.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gldrqugxk.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gnruufymq.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/guztddleg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrlibaa.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/ggfjzpbdh.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gdktglgpj.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gmroxpbqy.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gkdtpgtrc.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/guqsalyom.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gwedifdzh.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/geqynebwo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gwqboyxzw.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/ghlwohidb.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gncagsqjm.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gfgtmwyfc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gxqgwgmjc.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gpcgtunvk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcmffaj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/giynotfvk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gpfccjkup.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/guakeufiw.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gvzqfolay.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gnozboyjc.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gqboouawf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gfbxjxooz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gesbvhqlk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gshlwecrv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gaunzxmmn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gqbdvivhx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gkzyhinsn.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gxilmtodr.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gnhcieiym.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gdmifhyra.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnbufkjk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gvixjfybx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gfmiiftta.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/ghvjdtvig.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/galozdehw.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gyfhthpfh.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gfpnbxvip.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gnkdveqtw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gwothtfyk.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gbxqxnmda.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gwgfsrndg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/guxfxvqvy.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gztvehsfn.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gztdqtzbn.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gucnvgtkg.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gqldknapb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghayxsnek.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gpcolgtik.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gqznycnqn.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gslvwchdg.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gnleezbhi.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gimgymbgm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gbdzxxkvc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gpxbmfttu.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gdnqsgygv.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/geepkamgy.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gmkirtvkh.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gmnlkvsxh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gjbwbksof.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gukftyqkv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/giwramenv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gqqfdazjw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gnuzapere.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gbsmkgzox.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gopylbidp.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gopkjdlbb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gorwnyqqc.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/ggarutwlv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gjmleybgt.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gnhsaztgb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gynikcxla.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/grgagxnrj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqlmqbkfy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gbjloxggj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gtucibcke.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/ghgcsrlmq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/ghdmpxltu.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gkxpvbcgt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gpdfxfmkz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gvtgfwbjd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gunvellqn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gprjwkpkf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/grwojrjtm.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gctenjoai.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gxwjohqek.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gswftmscq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gujelvili.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gfpmtnktn.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gxunhbbla.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gbjgsoapt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/guakamujl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/goftpwxfz.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gvboxvwyf.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gfpmdcixg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gkcvzimnt.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/goarnpmao.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gsgbnezqz.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/goruyjwei.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/grkilqokm.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/glbsrxqtn.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gnajhltrl.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/giwvunamg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ghmqtxlmz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gccddhona.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gbmqazsda.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gaknhdkso.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gxipqbyah.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gzbwgqwgo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ghdddurdi.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gvpntqsbs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gnlqxcmti.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gybxuhivw.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gjiagkalm.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gdyboygfz.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gbunvyshz.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gaaekvccm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gdkfqwiwk.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/ggalsekas.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gehtftqts.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/ghuqqzvxz.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gmohzmefp.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gokvbaohr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gpswzurjo.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gmxzmgvfk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/grrkdpagz.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gejkjvtzt.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/glckoiymm.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gmfpqkagx.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gkuncrejb.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gifqfwjec.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gjeddjcmz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/grybbvfdf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gnriqlfge.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gmzkewzew.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gojsdaqga.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gnkdoteyt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gbyvqoojo.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/glqfletfd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/ghmiaugut.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gsoffosir.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/giewokpzf.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/glwggotui.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gvqeaoyfx.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gjftyruqa.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/ghwruntpp.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/glnkllkrr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gwfnikrvc.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gqavyblcc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gmustqcbm.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gaumxbhty.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gydfhfpkb.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gpnivabzt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/giakfmvqe.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gclicppro.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/ggdkcyqmm.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/grkhkwvhg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gapnkwbet.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gnvwbzulg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gxpicxbnz.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gvamhjnni.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/glychikzh.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gnkdwenzg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/goxpqyorf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/glltciolw.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/giwcbzefm.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gdwpfhmew.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfouyyxrv.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gkumoorxm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gufhdjzsn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gewsjguqx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/govxjazfy.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gxjogpivv.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/grpsjqlse.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gwfylyyyd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gnoxpovqg.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/guxrklpkh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gszqokkwg.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/guypnffnl.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gsigoycyn.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gdpfmokgm.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gtlqfkmva.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gdyphaasu.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/ggjtozlxm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtmenidpr.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/glvfpaskt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gppnvxter.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gseorltaa.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gqxgcgqcu.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/geflrcixm.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gpemgfjtc.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gncyqezip.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gjcygiwas.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfhwreuzb.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gzlltwhpi.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gooygxmur.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gpwagonrh.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gjtmfgwjk.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gbkuumjlx.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gfilinyso.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gipoxpiev.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gxstolmpa.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gfbmwhcpt.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/geajyiooy.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gieivopxz.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/geiqnowcr.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gjubdkayf.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gzebiwjao.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gsnrelhcr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gbrcewbar.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gabltitrd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/ghrjihoae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gsmdeawjl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gibdgijlh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdsynmxpb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gubetobgt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gliwjqhhe.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gnqqnlwag.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gammnnbao.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gcrcaqwkq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gisclprii.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gpmbbvlgr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fehbvm.com/Article/details/gjlhlalbu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/giprsavzs.sHtML


<!-- 参考信息 -->