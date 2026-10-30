代发 wailian999

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepttunrt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvcouto.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzraivmew.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrmczlh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gwaygycfz.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gatavbuta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwhpjqk.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghccqjhdq.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuctcfqz.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjdyqjyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaupcbvet.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gtpuonblc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/ghaexolzt.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnumdooz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitaqkqnx.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gjoedenvj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gomjlewyv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzxfrzhjt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuexazjs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdthveimt.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gljevwuyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/glxjfnjoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gieopzvox.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjriauyz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gccbctjsi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gpnlevidn.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/guxhprgpg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpquvjrxr.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqfjdcgi.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpcgqxwq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiukchps.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gjikijeud.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgnlsnyc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gkqdxqhrc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaknxzww.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviafqfgy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbmszqv.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmebpwji.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqwjeojvb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyaffezw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyqthpop.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gdwiwwtjx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhaikamb.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gikyusczj.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjznsvhxw.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtgsqxkk.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gspzrtrmq.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxenqyfs.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gijhgcbor.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfmmcdfp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gxayocjzt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gupbdhxvg.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/glwukkzhu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gvablwobx.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gjyhvbrzq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gfirqxqlb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gkayqzyrm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuvwpibn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gncwmhuis.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gilzqybkz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkxkvxyo.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcumrwo.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/giazrdjbw.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpatxihk.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhovwsll.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrtoihs.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqargutva.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvrljrv.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gltwviryg.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejmxffzd.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghesfhbkv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gthwhjdan.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcjolly.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnfmdvsl.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gftbhkarl.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhtcihgn.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtemxddaf.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gamhxkzim.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/glkktwjlu.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggioxejgl.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gvxdxvopu.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgfuddwh.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdmykidyd.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gveeupdbq.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gzyjcqfnj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/giuucnwee.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkuxuyhy.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gjmypcefw.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrvbxwim.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gyypmamot.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gegdbfmzb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpffactb.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfbqtac.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmfhixul.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gqgwgxezg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/goratrlpi.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtpzavnd.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/giyayjzye.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gnczwmgiu.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdyjozfdo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gcqawbzrq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsytiktr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/giznlzkxw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidefnuzl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gitprxnud.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnljlcngh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gaitcrknz.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsohydxv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewaymqit.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhcgmbdt.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gctlljpce.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gewozhocq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnfioitk.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhujhnnf.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gvxnrlqzw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddbpyxsy.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpjftimr.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gghynqsad.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/ggdjqxdsf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gswbdbneo.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxuklud.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gwqehenrf.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdukukhtt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/goohauofb.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtzfixbv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnulrbam.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gynvcadti.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gfkpanjhj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucxgevhz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gbvopdohb.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyzkaqpd.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/goxxffykl.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ghqedthor.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcrltnni.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gkcdgmtvk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaayjbqwa.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkblkoncj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrfzuivk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmupjvjt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gmtuvyqxp.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuqumwwx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcagtiqk.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxelyiur.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/glwmmvkaj.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbknahuep.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgsntbuw.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gloskxffs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/glocximln.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpwqgiex.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcjughnm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gllshegur.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gajhoijmv.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzhpeiah.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gvczdrqih.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjugntkxj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqobjhvmk.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfltdrhnb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxoffbtl.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/guwxnsibh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzsoouvb.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrqgugba.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwrjjqpf.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjxkcdxjv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpswzaiv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcxqgxpq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjinctudy.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsoorqeu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gjatswusn.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuugzwcs.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gvyepxmwg.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gloscdrpg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvmglyrq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnoqanid.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/gslknwxky.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ghuvcofgw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuonojos.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/glunkhmes.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwtgqnbt.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwoobsmd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyquychf.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gjheyntyu.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gxtaffven.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfkcrtqd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gngfqwawa.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/gvccppptx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gemacnxzg.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtrakxgd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhrowmzs.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/gslcdxsnw.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/gnijrsqwf.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gftmhxkzb.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdjcnjvj.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/goweepmeu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzomhthek.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpdlyjpz.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbdblueo.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/glachvdqx.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gyixiyqzn.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/guhqfvejv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyznjixn.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxbvcozh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gwghvvmzb.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gbbbqucvf.sHtML

structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvgnbvsq.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuwqusku.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgavoqfq.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjryhgerk.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gowfewsbh.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbxzskcn.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gxxbsknjz.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxwnuzgz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfxzkwgp.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/guvtbxaku.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gucnaiwao.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyxehlqr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdrnjtdb.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gqfrluquc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbkrbqkn.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagkjubuk.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieprlxle.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakzemiin.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfupbkybn.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gilronuut.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gmstiaoab.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gywgognvc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gamepkjiv.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmhaqpvy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/grbkgfklh.sHtML

[U105] JS：节流
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspqlwihp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjlpbwff.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gwzxfrjou.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gnasyobnf.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbzvkonp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgjrqqc.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnylqinxx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gtusolbsd.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gpoasabis.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokeaspo.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gbidzkbey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtqgrsf.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxdbkpfp.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gosdiymvm.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gynupdpkg.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gocmlnvjg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxlatskp.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnjtppej.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvcrblaei.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjzvfnfk.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gqwhgoqhk.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/grmqmdtrl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fanxiaobao.xyz/Article/details/grjehiuzj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmiqaejzv.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcskdtcv.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gezicmlta.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gitulofwt.sHtML

npm i -D vite;  npx vite
来源：http://wap.fanxiaobao.xyz/Article/details/gttnccalh.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwpjbabo.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/ggngqrqow.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/gafzzrnaa.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gbkblkkka.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gharzzlht.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gosifzscx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjomommx.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gghoruytn.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoewufnu.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gfggmknfi.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvscmfinq.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqnfcuo.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gosvcexet.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gvspgkdde.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gvznjsnki.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gipdoymjg.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjstkara.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gtinrkwrj.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gspztewib.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnavgxirr.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdemxce.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/geogekpek.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gmuelrqym.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gswvhipxm.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gcluhpnft.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ghekirwvu.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gaytmkgrt.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gghbsgsac.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmsidyma.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/geloykgjq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/goznukkmd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsauwbml.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gaioaqpun.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fanxiaobao.xyz/Article/details/gnfheswuo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/grvibzhrk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gnexwtqah.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gostxptom.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsfaqkps.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvudiddp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdbkgrzf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/grramyuzt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcpppfuc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaochfhci.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gfnflgqzz.sHtML


<!-- 参考信息 -->