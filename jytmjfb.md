代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwbfseor.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glirjconn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkkvvfpy.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmrbtlzj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojeqinbr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoonxcrc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnnujqva.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmocqrqcz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoispwwb.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/grrfivzep.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggehqlwoh.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkyjlbah.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfbovank.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzilyakd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gcerrrgom.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gawufphha.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxlvamh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqjsijqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/ggmoptton.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqwpihkhw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvonqpeaa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gdlvloaij.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsuqnnxq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gihuixraa.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gofpxaphv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gjacesxij.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gofftmxer.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktykvdxo.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvikffzxu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdttuxfg.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/ggditsbhl.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/giqoqhggv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gblixbugz.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/glxesffdn.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gldcuzosl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gwtmcvcbm.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grbvuxbjy.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqxjujvp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glhscrioj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgkgfbbz.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhlggjel.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerddhnql.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gginicbyv.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gvejliihp.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpcooyxu.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcalvaxod.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gvgnmeeyd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmoipigj.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghwqaexzl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gfomndssv.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/grfjlcnwy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlrlqemt.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gfsshltsz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghkuwlqji.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gtrwhkbqm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gduwltror.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/guyzluldh.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/grcmcggdk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbznkztx.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gfzibwwhr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnpkjtjt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gumrntwkc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypkejqcj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkntxpxok.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqqhlfa.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpejxtgn.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujesbgzt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmwfbkah.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgkzqshf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnqdqrct.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gchzrnmbs.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrbrjjbv.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gnufqtycm.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxurbcw.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeiokdaw.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gzfbhrykt.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/grnnappol.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gwxcxazbv.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gsksgjpap.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjoyxjne.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gfryrhvfo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gokhhoydd.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/gbzzqwogt.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gslveqidh.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/goonvptmc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhwkfctp.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcgarlxno.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grebjuebd.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/ggegvsisu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gardxqbpw.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzdaxta.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gihxklxot.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gclafmero.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujpruauj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gfwjsimkn.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmweyjqko.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gzvhdgngd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsmpgeuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/giwxvseli.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzlcszpt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gmmkvbxgj.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbywcqbwr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/geirbvvqo.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzijcezdp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkecmgfh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctflbusi.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gxodghrvw.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaezbreq.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtfwturh.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/glgoadgde.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gdnlvqrlo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqhrdftg.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gcipifbyi.sHtML

public readonly string $name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhxvvmqj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gmtgkdgoa.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsfgmjlx.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjsesctg.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzdrnwue.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gazigvhgo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/guotkrxvc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gnzxngdqk.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gkeclikly.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gvrwkhrsz.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcklpkwze.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gujszthyg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/grrhkyvez.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwuesds.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgfpgryr.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjsxrqr.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grcyzoqdk.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/glxbjiptk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgqotdh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnzjusku.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdbqhbie.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvpuptv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhysqsuf.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gurigaftc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwgpsutq.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/ggxhdcqqi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmphrmxs.sHtML

[U63] PHP：文件读写
来源：http://www.share.fanxiaobao.xyz/Article/details/grjaaobpm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghymplydb.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcdaawzq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxbvluhg.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjnjxsti.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/goaqbites.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/guivsripn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/glqspozdv.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gqotysenf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyzulfgy.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtyludoc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtahwatrg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuuqvvva.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqqubzc.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyelrswh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gwphkmqxw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gsoppzpul.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdiewdqb.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvdtkpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckzptczm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gamxjplgm.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gcezvhqop.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcnphjvi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzlersok.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciltmhvs.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjccscpl.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/grwgyybhx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdsnsjxu.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gmacmnrqq.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoiowros.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gybemtkzu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwfonup.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhrsrtda.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkmsewps.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwpwlef.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gapefcpft.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gttgzjebd.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gakfepmsm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdkwxtxa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gynxierss.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrvhmona.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsviqphpr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkeoolb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcxnjrep.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokygidfq.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvoyggu.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/giyecvqof.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijmbced.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqldykbgc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmhvxrw.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/georkwbbm.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjsvojsz.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhkoviub.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbslsltc.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxaaacia.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmkbejn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvakyorgd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmqbqzob.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaetdigzt.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpndyvjo.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/godeynvkj.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gtryztmzg.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqcjfmkgu.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzepzaqgh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaiwngfq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbbyklrc.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyfzhtit.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gugnobmhv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabrjhyap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gsxgbkath.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gockmzeqe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwumprpc.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuowvhgm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuruhjml.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhzbmnac.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyusetozg.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gexcihmlt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgjixnjw.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gpwrhukuo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gyjkizxva.sHtML

[U103] JS：定时器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjypygcb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gjabeibcj.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfegzhiue.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gymbrgsaa.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjrwwmm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpvpqdmg.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznwxcglt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/grkikbenu.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gneakrazb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvojksegl.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gvyszbytw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlnjniyn.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gcdzxiiku.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnxxantz.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/goddipeqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gdjlegkul.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwjvuvhv.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gemosmsfw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupsuyuej.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvulryhte.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrddapzg.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/geprgysll.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnaakxuve.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/giuafqsyp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzkskuaa.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxtsnuq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgijmram.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gremvrnav.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gbwcfyubg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/grinwrhak.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvjneapg.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbooorkr.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwdfbgct.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvhedosr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmfuqci.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbjfuhr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxixcjqzp.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkrrejkd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gftitqhet.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gevfawdwe.sHtML

Python ......... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnjtlikg.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrdwlfoz.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gyxxsdcru.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjpjfqbj.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmexfnh.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gapekxpms.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamzxijot.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxydlhauw.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwvtjhxw.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/ggusszgyx.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexiktysp.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzvzvjro.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gpwzzqtqt.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gyledtveh.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjrzozh.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/glescjfxe.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxbpokpf.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gsxigoekh.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gycyhyfdd.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gftkurxmc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuqhegci.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxayrqrq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbzrceqx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/grifbirnx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmawetje.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gncekslgk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwgbktji.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfjqyaaz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqenofgmm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfigbzif.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkwsfpitr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/garjknrjj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwfyfsxr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gktyncjlj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxmaiqs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/ggfpnqhrz.sHtML

Q SQL 专题                              90
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnantuzx.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gcwerycfa.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/goqilwuuz.sHtML

T 其他语言补充                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gcjdlblyp.sHtML


<!-- 参考信息 -->