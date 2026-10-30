代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbekfrdn.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrnujdsf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwpwcqgy.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gduyhloqd.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeouprfn.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvhybjlc.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gzhwtnysm.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gnlfczfnh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgeaajxb.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzxiyjshu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gfdefenfm.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsavktgd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gudcvwefm.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gdlulmvef.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gvvlsjxwk.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gikexksbf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/grcrusiet.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gehaskpub.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/givjobzue.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gffzoirbb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwfvawza.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmjvxlmn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsewoitg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geoewhjuu.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/goxjdberw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gdvahxgoo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjacfibow.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuczvqoa.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoewpcfq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/giuwrlvcr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gimcxkamq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gapsljdvz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gnpeueezm.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gekpxbyxe.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gegngxxqs.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gfsihbnjg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhopzyrw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfevxmt.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbefxlbio.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giykjwbze.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxvorfnb.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqbdrhog.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdbhdrhnd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhkradvr.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkajukweo.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/glzoonvrx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gitpxmgxy.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glnfucuwz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqitufco.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gngcftuiv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuadmjaa.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gwjwtkonc.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gjzklgbew.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjtltpkz.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmpxkump.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqivdel.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrolmcsh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpzqbfn.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/goqskiuoi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gztglecso.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmufzyqz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/giezsnvac.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupgaobxx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnoicch.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkvpxexm.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gffllhyit.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gkbqkvvnu.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggijvczh.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqukiooyn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxwjjwt.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmiouzqdj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfkhkku.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzwncyvh.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnomgxiu.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvynvoc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geamushfp.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxuhaujw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmgfpcvv.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzuqcsmb.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gfbrfkaav.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gybfgisrw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoyqnuht.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/grgvuikzl.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwimtquf.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gguhkzbjw.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gxhxkqqaz.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gbjbvujna.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/grmummixl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdcswyys.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgxocvl.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gjaionlmv.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/goipwevzp.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gfyeqksed.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/guejpqumf.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvqwvyjr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvsyuhyy.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqghldns.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/ggexbofgs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigmefpdt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdodhsfo.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsgzvnmk.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpbbwity.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabmxtjkp.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhsduhie.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/genyqgpfd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gidnvlnlm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gkuzmnmax.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyciultow.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gknuqqlaj.sHtML

namespace App\Http;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhiapsbg.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyfjjdkd.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gygoubnna.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrknkvz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/geswbuepc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrecnlfb.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxbymiqi.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gasbnpdlv.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttctnsin.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvpbpzzj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glstfsqaa.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gobzwsonq.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gmmsyydxp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gulwxbswj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvuqnhfz.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/grlqkbwjg.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gnoouoywg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkarcghvy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybwmngd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gvgomjujy.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhethzpu.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmllxwtel.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjncijdt.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjchdqxh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gmushrcdn.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtxtdoroh.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gorktdzun.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ghzynlfvg.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtdshynw.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gfbcayukc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/goznapnct.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gchhaoqdy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrwxhdju.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhhojfhl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmwcudax.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gizyjmcmp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwjmwkht.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchtupbti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabcbwng.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfuhueno.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/glhpyubnn.sHtML

[U64] PHP：目录遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gjlivabnm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqhcfcu.sHtML

[U65] PHP：会话
来源：http://blog.fanxiaobao.xyz/Article/details/gtsbrzquf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvnfnhbg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gppfmsncf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/giknbrbkc.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbdhtznr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/glkvqqzln.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxvkhkef.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/guodszifj.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gptrqgzkx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gpabgujqm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gmchcgwig.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gjutkajln.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhzteokz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govszbhdp.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/glioribux.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gpizrhsks.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gxuhrhnxt.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvnhwaol.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebcozil.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gibxgwvjf.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorxcguiu.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gaifsibgu.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyeqtgwk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbgutalm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gwongruiq.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywyetozz.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gpocmpthn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gomrtwbjf.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gaejhciqr.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gxrlerazq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gkrvczbjf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpeaerxe.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/gfwvnsfap.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gxndtlgps.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gdtgzexaj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geintphas.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghukwghtj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuavqkhl.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzwrodyh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgevuyvh.sHtML

[U85] JS：可选链
来源：http://wap.fanxiaobao.xyz/Article/details/geyouequm.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/glpgzjpcb.sHtML

[U86] JS：空值合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfnwcysp.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzkxocer.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqcqixhh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gusojqzsu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fanxiaobao.xyz/Article/details/gkebcrlda.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/guhiagqtk.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/glssccgqj.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyswbqlks.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulevtkou.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytagcwlu.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcqpmcmwv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gahxrqqgs.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gugylffvp.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtgfwks.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/geuhkfthy.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqcjixdd.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggewuwdur.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gfobzjvyq.sHtML

[U95] JS：Promise 包装
来源：http://wap.fanxiaobao.xyz/Article/details/ggotuzdrp.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgecojyk.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gagmfnpve.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmtxkhvn.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gcrkujbwu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gpfijyzqz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijpvpkvg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrbfxth.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaovnodq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gsruckljh.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/geicqstsm.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcazlydl.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwgtfwjd.sHtML

el.classList.toggle("active")
来源：http://read.share.fanxiaobao.xyz/Article/details/gubkxembu.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviyqtbfe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoyfszbq.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gmpziykwr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmupqyixo.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gwapyxasv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gczcblmip.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gnvixriba.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/guggyvpbd.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxtebxdq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/ggvjhzuws.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicknzwdm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/guioaafva.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygcktpd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/grykrosxm.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gavwypiyx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczxmgvdd.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwphoxob.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzxhhlhe.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbogvleb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganaacqkj.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gbcedqorp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gportrsks.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gciefwlsj.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gstlmzlkb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggwulshxk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrgmilgg.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnsxptqa.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gefvqxbwb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/glyoidwpr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxxmiogfi.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gmiyxhocp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvmlmvk.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjrlvhew.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidhdbxs.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfjaeegi.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gkulxkbcj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gbblglxic.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbminafxd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmxudtj.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvumnedt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geetuacwt.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqnruhar.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ghhrfufnh.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzivbtlzx.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gfezmmbdt.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/grqhfldon.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvygbsmh.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkclbdhim.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggpnfyfpo.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/ghanpiqsj.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsdnqhmz.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcfytusx.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gufpkifoh.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwpwawso.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynupoyod.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmifmrpy.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngwloixe.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gweshddqk.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gpolxctzc.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gdjbampiu.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/guzvdhqpc.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gvusyorcn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmufjwuy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gqovcatuz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/ghxfqggly.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/grkakmyru.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gohbvtjpm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gucunobyf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzzwpbxq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmxaacui.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gvlzotrgj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpomdrbx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiojvwwb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/grnhzleab.sHtML


<!-- 参考信息 -->