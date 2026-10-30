代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gobotnlzj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeqosdft.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiyvhfuf.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnnooxqg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszfniacb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhcqlntm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gjkcnmqqt.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdiafddp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiynenqk.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gbmxovsmu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhlnquxx.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/grnnagtsw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gmuyyblxm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glymkrzdy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbqnznfl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxnghjhn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/guzojvobk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gomzukfqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgrllqxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsxqfdno.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmmfrzal.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ggdwcjema.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gzocwlcge.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzokfofs.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbitrbhzg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjqvwpkd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoxjyess.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/guxbfsagg.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhepqfkg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcafujcgl.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqgxejs.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/glxhfmggo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlwugkk.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/grvkmnmfz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzuiqmkr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezmxfvev.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkvkepmty.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmulcvrc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guotvgpmu.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvpaipah.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjewhklyq.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnggjrndq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcmqdochq.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqrtmji.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gyhbcswwu.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ganlgeytn.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdidsqxe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvxvygm.sHtML

[U17] Py：初始化日志
来源：http://3g.fanxiaobao.xyz/Article/details/gmphtqchl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnskrbmf.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gtmbqssaq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiptnyjk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gogrzaxrw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwfitwevc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxshwccm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgujlnbq.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gcipyqvcv.sHtML

@contextlib.contextmanager
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvimtwze.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ganhxqmhe.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaumzsofk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqstyxcd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giedzuaxq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giprtyevh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrtfdcla.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjhchgew.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/grywiqdpa.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gncpmxzki.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/ggsviliqv.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gryhymrst.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gpgjhyngm.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkvfjkpo.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbefbrad.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaofkkjog.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gjtjvetxv.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrqzcmto.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdmxscuy.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gybpzpaxb.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkeenek.sHtML

[U32] Py：代码格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfqsverrj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gtycvipmh.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkudwri.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhiatisk.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfrkqvke.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxdmhdyp.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbcnprjp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqeesgin.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwwkpzzxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhhitny.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gxqbhvgyh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/ggwjfagoy.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gasvlidnx.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeurxtvo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouqntkwz.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gytlxjzgk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gtacdnlai.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gupipvfmg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzpjjahh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmtollkb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/ghaxlsrvj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaiisbie.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvluiffl.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcscqfk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbvxwjvq.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gdckbtbyb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwqjzyopw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqnxlqv.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvagmuxl.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gxsfnsqvl.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymuazxbc.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuhlhnui.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbtxvhcq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhoaayyv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmcdekrg.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/gpypbnbah.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqxudqot.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/genwpwixj.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/giaezwphd.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gecbsoule.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjsmrzbbv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgkhxzmy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/guaakufxd.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkmqwyro.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclryxmvj.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkojaeyw.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrpqkxuz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gxvspqgdl.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvanvzgs.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyaeivxj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwzpncaq.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkjnkhpb.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gmkjkmxpb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklzaulpt.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqyocbqa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxlrikyw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/goinhmfsl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gvhezzfir.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ggczchyqj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbcppfndu.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gifjjbinz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjrbsrbl.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqexayyuc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gqdqmeltg.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqnudimrn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gvajcgoun.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gbkqklurl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxcnvofm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gqapbygqr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gkwvxumxi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyriwbp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gnabkomxx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgrrgtyx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/geicqvfpm.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwdwdlkwx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdowjjzkm.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvswbdyn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhejjapd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclzcwlh.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gxkkjlnne.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/godaqvkkz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gytfqnloz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbzppvqs.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gmucldpop.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gatmxgdms.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gesahcfhx.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gfcfcnapf.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkqtlmlu.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gwsupztyr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/ghvmyvmpg.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gahkahmzo.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxrlxadj.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfeutlby.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gipewuyzz.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gjxioiwek.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwywdhmar.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gvafstmdg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gonvbvejc.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjodmmbni.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gihjxzjqt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gqwegqpyr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmepfula.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/gqgjwsewp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsnmowgg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmedersfi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjfcpux.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gmayvxqih.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/gbxrleiig.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gtaufytpe.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gzhpzejaf.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/giwfrysot.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glozigabo.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/guhfxaymd.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxdkxjjh.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiwdatys.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gqjhfrqpy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbidegynf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwlpokva.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhphulxv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwxkowjo.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxecaozws.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqrsxwqk.sHtML

[U93] JS：模板字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzasbmaa.sHtML

`共 ${n} 条`
来源：http://baike.fanxiaobao.xyz/Article/details/gangtzkcj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpclzyv.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gidwwhxih.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhfelqvp.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtsbjud.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnumhdzxr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/guapvtzuj.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuhdzjyn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gicwetvgv.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gcydboilz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gfcwhzobl.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfhficrl.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gklmxeidd.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxcbicqwy.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtkmoga.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyurlfgyl.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvipbtneh.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/grhawpthj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmansksvp.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gozbxndao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhbrwlvo.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkocwcgo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjklzybqv.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyarjjgj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqlvdqfzv.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnoazfjn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiouyzlg.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grcmuittz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhqarbqv.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/gvksrnuyp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gkjfwiptx.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gbudmrghw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdcsmphx.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkhljtpu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfixrdz.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkznkmqxb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokjfzenh.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gmyqrmkgo.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gnkhlaqdm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwhapxp.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gztmwfxtv.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrplvpps.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlefhwv.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gmktyfdvu.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/godlxifvw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbusnskws.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzimwbjty.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwdvrxao.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjxpyahx.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gclfipuav.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gbkpndrft.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gdhfgpzuf.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwmxuxda.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gwearznjo.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gweltbaoe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvjtfmghh.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcqkgem.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtcrtzxdm.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/ghreuzvab.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfskqdzw.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaskfenb.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhbunehy.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgjgrnwh.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gekiacsfm.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqjuuujsu.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqdceemm.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcjgejh.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gysfclieh.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gttmutjax.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvqciyc.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gglmdilxo.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/guipwvotu.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gmsojpfuh.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gwljbnymk.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gnegbolpq.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gvmnsrjck.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsputkeop.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gwfttnjui.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/giltcjqxm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvjmlex.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchgbouwg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggvotgevb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpansukn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gmafesbsh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqxadpch.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gjglcjslt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gfhxbucuq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyydvtlmb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuholspc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmwmugif.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkqkguvtg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnsbcqhs.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gnlshuqbp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gtjbrqhpy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmldcxpy.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/glviavvxg.sHtML

R Bash 专题                             80
来源：http://wap.fanxiaobao.xyz/Article/details/gaowckknz.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/glgktsygp.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gvccaxybk.sHtML


<!-- 参考信息 -->