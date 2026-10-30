代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtepmhdi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydxkjdet.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gxthqjrmf.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gulsxzbox.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkomxzwtc.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpxgmhkk.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ghglheiml.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/govtayrmg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsyijohe.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixuucbos.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzyllwpph.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzzaubot.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybpqibew.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrloriyb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvrsodge.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcqjcpsh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqxdcsla.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwxlahqw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyujlwj.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/glheoukrl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlkmkoqv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfslvjms.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrlbrmnh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geodpbhtd.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjnmxxeat.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/glpzxxrzg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gymttcenb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gomeiazpi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gtggmhmnj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fanxiaobao.xyz/Article/details/gioeuqsls.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaomzqxa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkytqetm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gurckilnm.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/galybpxxe.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gowzhivaq.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpuwbwmb.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvfbubag.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gmnykyzlu.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gqejagpky.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gcgfamcbh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmngmpefa.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcixpicwb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfjpgov.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/giunwpcam.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gogjnuipv.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxnbpmdbo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/ggmpxbeti.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gboqyzftb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gilijewgr.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gkouveamh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbphpgysw.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzhvnkme.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gnlgpwlnk.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gmjjxboby.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumevrfo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdoidecb.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmzbhkxh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzwqisir.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gnyxbvesr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeeyhmrn.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmntjiptv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwgtjioo.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gijdahqnc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgxngpqq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiyizcmp.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gysyiomvb.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/grsyyctok.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gskfsxrdj.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geoeffkzn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gjggrzhfv.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwbnygfi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gloxcohmv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gztekfpwx.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvidxuvn.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gptxonrxp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvesxlebp.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpkrlqwm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gqvncxlmn.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gdkifngxw.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbuutgyb.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcouxitd.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpubgiyk.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwjwxokj.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxfglwqa.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/glqpthaig.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurcrzzoi.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/guevzibos.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gmeiadzky.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gikoujcqw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqxiapzu.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gewgbzpiv.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gkbvmrcke.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gdunphxox.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwwvefxj.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfbgjbca.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcgwlwhi.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/ggtishsip.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gofqjdnin.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gvktrgiaa.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaqcsgkv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gfazdigva.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gpskdujso.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghehpsvdd.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxmutgba.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdpxqvf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfnzodmt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyxkogok.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmmvgcqj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gjlpgkiif.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gyuoazotb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grvstnsrg.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/ggulnxvtx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmifvtn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvftdoptu.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggunsxcsh.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjajqfb.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkjemlrvv.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gxmikvgje.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gegpetbpx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gigngpgoj.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gwikwoxkq.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakefuuln.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gbtffjgsb.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnkqwqvlu.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gfrskzadx.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfbcqdtl.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqqmsqdq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvleimizw.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/glhnnpxxk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/grdcjoygb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdnpwwlv.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjocllfy.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmyyjbng.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulsdbmnt.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gipkexuxb.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaftcjtsd.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gnxzsvvoi.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gegsypsxe.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gsmvjjweo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/grgzhdnoy.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gtkdlurkh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/geaynyqgj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqauntmzo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gycdirnpb.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyjekkzd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagbbmrm.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkmjarqr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gzvbprnbg.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gekljxxfr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqulwqyq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkzxfvbn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkckszeop.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/guoulwmoe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqtymdoyk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtakkccq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/geiwomles.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gpliqfbsy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfkccjdo.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gpisoaepi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/grehqucsg.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gojlgjssn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghqckaarp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyqupnkrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdrrhrt.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gqwyvwxkc.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gookhgoyn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgljkvcn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgffioht.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gudbhqsqi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzpeudgv.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcarhrguv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/glyvgwqvl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghggxovvb.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gevnmugwh.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gysudomxq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gducckxey.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvlhocaz.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/glqivjzmi.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gacadjymn.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gwthkkvew.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaxxjvgs.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gyvkqtbbp.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmdderb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gcdefberf.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gcnhlnxkr.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/glqmaskst.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gblpcuvae.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gbvinrxhk.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdwkules.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnyfavyc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fanxiaobao.xyz/Article/details/grvyzcfyy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgdthwht.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gtuqxkhhs.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwhhunna.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfgkruah.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/goskelqse.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/goxypbkfs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerximzsz.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/grkariwqn.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gharlcerf.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcwmfjmd.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gpkngmgrp.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gihrwflft.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrfvbou.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaphhyryp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gnidawjee.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfkusvgdw.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gkvgrpmys.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlsaeacc.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/grtmiebau.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgztzbfb.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcltzfhbl.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjincnh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdreuaefc.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfxobugk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgiiyguh.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/guqdekqwe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gvjdcpdoi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsaqbzun.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gsktywvuu.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkwyzvev.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsodvlhay.sHtML

[U100] JS：DOM 查询
来源：http://wap.fanxiaobao.xyz/Article/details/gimomsqfu.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gsxyevhef.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gervtktur.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrgkxwdd.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/goybiuskq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjlfllkb.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhtkhde.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gluwbhhuk.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymgciem.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchicotlo.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzhwamnt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/glbjftkvf.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzanfrupr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsyzlwfv.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gietoxysl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gadfoymxj.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrejsbia.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqvmduri.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrsqrmej.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gleesniwr.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gclkrijoq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/guipmuopc.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdtforym.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqvfahgu.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/groezequy.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gidkdhmyn.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gnywlkftt.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/geaxunemt.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwszxtmtj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpukfpfq.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjdshpsk.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwrkiijs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzejxjah.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdyntlhos.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfyrazvm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gpqoezexd.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gstdckpax.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gmkyuhzkw.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glldpouxb.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/golaccoen.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdrnyxod.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gszajoqsx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvvqgrj.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gloetwtev.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gowohfnwu.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/grmyvnedo.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxidtspw.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/gaqrozfwb.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjadjqic.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqxiygh.sHtML

Java ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrxktteu.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjphekce.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgjdubnk.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/givupqwwa.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/guahigpbd.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqamtpnk.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gyvtwhrfx.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/giujogcjx.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gryeudjhb.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gspomrufn.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gojnmyaos.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxowcno.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbmaaig.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gquajbzoq.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gqarazdni.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxebwphc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gczdtiooo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrhudolo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gacbekspu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpbahed.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gudtgdbqu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/glfatdfim.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmejegie.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjpdxmps.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxgyfcah.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/grlwpqqdo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzxswjte.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmgcaeas.sHtML


<!-- 参考信息 -->