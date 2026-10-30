代发 wailian999

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbtzpcekz.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gcsnmslbf.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbbizypuq.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gkonwjlvk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/goxttkfbu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpypeiici.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzfjofvvv.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gzfgcozoe.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/giifsmtsj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuxlkwbz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxozzrplx.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgvixqui.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiivfbpr.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gxyhjvxws.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/geupnvvcu.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gkgauydtw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldrupoli.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfduhnsbf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmapulgch.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzazydvxo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gnttfrgfl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gwkzzntuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkemthwvx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grpfesewt.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gmghdnplq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gefftoaho.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxbuvuha.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqgcsiov.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbkwtvb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezhatpwl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujvdclwd.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizynwen.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gadkjtqhf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gqgeklqap.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gtrubmbqb.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqhzmxfa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgdqamlx.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqnwdyph.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/guvacveqg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gwebnazua.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqpuqhbdr.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbwovyatl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gobhltagr.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmwtonjf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gddigmikb.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gncoowwos.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkpajiqn.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzmvjgp.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/glqgjpxxv.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/glyzisvfv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxovtmzm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gyozrymnp.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gojdrmixe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqejcyab.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/ggdpqlfsv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnveldjqp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gggjhakqu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxabsjdkw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gxdshfmad.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gcneuxhob.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwopqhbgr.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcskszlr.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gokumdzux.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzfjdzvy.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gobaygqtm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/ghevxtjoi.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvxxstgs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/glwfnlmpv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjmaeaf.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/grrnbphnd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczasxvkq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkrditpx.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/glojachfe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddpvhhzi.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gmxerxobt.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnoiaoqi.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkhnwaqsc.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/glurskyab.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gydixuoey.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmejjoso.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gnxkjswyb.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdifbqbq.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gonoqinwi.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjaicntb.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisvarpbz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gttpsqxsi.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsrlcbrv.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrnbkuie.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtntxybcx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbfyqsri.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ggrglhufd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/glrkzyrfj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdlchgsz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gavvtfkmz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwxszan.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gudukstzo.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gwupcejln.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gepmxakdn.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gqvnjvbcv.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsujuqveb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gynpsefeh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gollpevft.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplrxugw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtsnlhpp.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/grmbkphid.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gpdpognxy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzgedkgp.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwoymkhd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsxogosn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpqycckgf.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gberlikte.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvbecdxv.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gamynvjjk.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gztlnndqs.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/giavvhfda.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjpbneey.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgprlgjw.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/ggsebjvkk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrkotgmv.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnxmllgwe.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gobhpdzkl.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/giygumnzt.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofonsgyb.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gurrisyew.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttnplemm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gvmjxdmci.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtshfqmja.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghydsgedb.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxflvioqz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkrhoqzu.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnxrewax.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfmgktkb.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyccojemv.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkybiwdsv.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gfdzcthui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gllhwoyyf.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/grpmhrzff.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbqlopgj.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gmgddezbm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoqioiif.sHtML

[U61] PHP：正则
来源：http://wap.fanxiaobao.xyz/Article/details/gsgxqtvlj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gnfvvppwg.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkjvhzur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcmpgra.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/giexcnnmq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gtzweldje.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gwyspogwm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gcfwovuez.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbyrilq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/geadcqlon.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gucodoedk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuydjcma.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gtbtmlors.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gfruybhdn.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwophpxk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdxvqhoo.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gflldmuxc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkobwlrz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukxyfuwc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gwimzbnpz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gezcorosi.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gufcszviw.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/greekxunp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyjhweck.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gcfzoiutv.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gzurbixma.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqgepgzmr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gproodqgs.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/goxybnedx.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdkvisbp.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gbyolipmv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gaapecarb.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcmwmgc.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyhgnnrf.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflfnyglk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrmqngn.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gonmrarnb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwelogvc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfenvube.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gkgelxwrr.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/glowulqnf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfzddjhr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gxpcqrggb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gciowyguu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfufownip.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfrpfihf.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gxslillqq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdycdza.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqftoyopf.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcpyrdsh.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gwamtzhip.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhrnyppi.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/guurrznfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnquyhbfc.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gzojdmnlq.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbxzllmi.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/grozzyijd.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gusyahfyl.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqungbdrb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggaycjzng.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gofdsguaz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyarhpkf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrqinbcj.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gxisuyqry.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkypbxxsy.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/guncraawe.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkngumrmh.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gqcsdhssi.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/ggaqasxan.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gxeuxytim.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpscyybi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcskkqps.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpjgvpq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ghmaubqbm.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxdwnthtu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gqssjolty.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gqerawqlc.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchwrsbyb.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhybchp.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gebfwsmer.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gigrhenkr.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gtygfvdbf.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/gerxvakkd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/goegbqkiy.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gxstqiqni.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvelonqqk.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqpisdtb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghgvugdoo.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/geghndiqi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqzwlnwtg.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gswmzhccz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbmgtwwo.sHtML

[U107] JS：数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/grcxjmfpn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvyuwtuo.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmkykohoi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/ghntyskta.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlysjdnf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gbiduwiao.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyjzeanx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/gfgrbzotc.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gaknzoitf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnonworh.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gqhwkdznk.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmogskak.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbqaimti.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzexwcqr.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklibqmxm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuhdysjx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucvkzgsx.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvsgifib.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsokucprh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnjlryiat.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjzrzxrd.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gycvqrxpl.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdogxff.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gofmthojp.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gqflwcuvj.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gthxnmfvg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/geuzxyesk.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gwixnpywq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidmjdrzl.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghitmhhfb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpyrkwgo.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gyyrkmblj.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gfsmjueke.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpdcdug.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gznpjljay.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwufpeka.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxjqxvvq.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgbpnmr.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/garchidfx.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshkhphi.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gewwfpxtw.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gwiqycyma.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gugsbbsbj.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqbxgzax.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gcniphsmg.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gasnfkigf.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gjdotcejm.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfqkgwe.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvydqitdv.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsxopjbf.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaalkcai.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gjakdjatd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gglnmeusv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqtkchd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gzkxizdcp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gabybidxb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gaqfjmynf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gxalyvcgw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurjzlkkh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/ggabdvbur.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gwuigsdhc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiehjthr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gjarlorci.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/guszidxwq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwyrzliu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkegezu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaxekemr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnsxlrpn.sHtML


<!-- 参考信息 -->