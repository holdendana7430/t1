代发 wailian999

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/geynqrmdk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxkszpqmy.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbjjmpffj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gzosuilvd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gimjuyews.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gmmlqkhau.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwcwwhyim.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gxoaqfplb.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gqmricein.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqevzbdrg.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwakbniuv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gqzfajakr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gbygxwknx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gkdodmpvs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gffppcons.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gchnijxzi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gzhjrfdgq.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gvieiznwa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/glavieieg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/ghjddxrba.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gvhmxpxxe.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/geiazvvko.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gkargvwry.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gxljzzdfa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gppgwyoln.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwqgnhbtg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gdsuihjet.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdnxzcqo.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gpbnjoiyy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/geiwblplh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/glwirkhld.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/glwxmdmhl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gttcofnua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gkslbunlx.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gweootjkr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/giucbsptx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gnpilpfwt.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gbndzgpyu.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gpjetpbjm.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/grinewaqb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gtjaiqkot.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gjktpcmpp.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gazfsiasf.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gpipekzcv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gejarvwbs.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gnyphxcpe.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gqdczszsk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gxewfedka.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggburgwwk.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gsfgzbatl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gboolhxqf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghtiahgbk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gejiipkxp.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gsaeutzea.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gvdeevgbc.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gonzncssp.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gpaiexukt.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gnwucjqdt.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gqrkdfazd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gmelorjeg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gnbuhslfi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gruzmzacs.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gsiaunwln.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlhnnma.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gdzyoqatd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gmrhzisav.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gajxienws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gucafgeyv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/glqjkljeq.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gszfsmwky.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gsympvmsg.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/ghcpzpzjz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gkmshcwwh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/ggynnodjp.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gfqzbpxjx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gzhqyofqw.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gvbokhrbo.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gaotfmfhl.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gzudvoxqf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gwigvgpho.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/glvwvjiap.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gkrqlnrou.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gyvyxotae.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gmqsvoily.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gacwhwkna.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gbyrcmbup.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gcyoaxpij.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gqbspivkk.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/guxdmknpk.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gutaxtkjq.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gtluueejb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/ghjtjkzad.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gomkvaimb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gpraglcvb.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gwdwefeut.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gsljqrqbp.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gmgupzcst.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/goabrdhfz.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gthuydpfm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gjdfojmwt.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/glqwleulg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gbjkbiwvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/guemzddfh.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gvyauzxcr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gjhrathyl.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gzxsgngpa.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gpzgsryni.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gahdxqkri.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gczdwdmsp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gogdovvkn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gkvflcosb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gmrsswgjn.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/glujbjjvn.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/ggudkywwj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gfgnqward.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gmlzzghtf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.zdbjq.cn/Article/details/giamdhlxg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghtvetnlw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gufsqhvip.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gnjcvddzd.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gnatfwtkr.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gcbegsiia.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gjqrbqfwc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/guqfcteut.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gvgujiyvq.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gwmldkfda.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.hesvh.cn/Article/details/gnfwvradj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gosyplyma.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gjpgzahzo.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gtajjcfzt.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gpvcedhwn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gkafjpukg.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gxjykvhhq.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/ghteexprc.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gvtevprqg.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/goksrozsx.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gqguyttzo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gqjvnaubz.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gdcfvbace.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/grhizsuzk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gecigexxp.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gwmtwrpjq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gflfqnlho.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpaoliobk.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gwvjfutvm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gzwqxvxmi.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gehzearxo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gerwnfubs.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/guvcjegtk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjvhzju.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gjjcuzfrj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/glylpuhni.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/gjtuxkigm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gwaqdiqap.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gidxtqxqt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/ghcrevsbd.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gvymitkvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gekmnxtfi.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/grksuhriv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gttsnwnqx.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gjhwynpkb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gweheqrah.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gnpcserzi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/glphonvmu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/glxtxexnt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gcltmjqes.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gcxpknrym.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gtffqzyfj.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gqjmgqvvw.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/guusufowq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gswqalixu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/ghbptpppw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/grecbawhc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gfflpbdhq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gfhqpstdz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gyumqqgcp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gmrfexdmk.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gfdfmabcq.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gpmdeeqez.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gnyiukyux.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/goqmukrht.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/ggjyhxaoz.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/ghoniniag.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gkswfoehx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/ghnnyhtxh.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gczqmdvri.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gyzcpskqh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gvornuxet.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/guuupssop.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gzrokwvln.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gagxoxxey.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/ghiekszjx.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/geswfozjt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/giowbstoy.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gklwypkrm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gfdpylagj.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gctdgpxgf.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gtovahbpe.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gdskxnfol.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gczsoimlt.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gqtbxvmfy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/glowizuvu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gakeiufal.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gxpubbduj.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gfvmsoihr.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/ghcwscpgf.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gwexclxql.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/geuwjfrkq.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gswcjljbq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/girhdcnwz.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/grcrvleac.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkioaoid.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gfygoesxr.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gngibdiad.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gpxeykner.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gulnehtjy.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gezusewsd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gqlpsirgr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gugntfacg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gswfdtlvb.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gwwathdxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggnpghtva.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/guenolluq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gtygcvdyx.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/ghyrcmgjk.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/grfclhave.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gavycdsae.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gnwjkxjly.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gmgwedofp.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/ghnmmkypf.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/glwcodnzh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gzbejsqnc.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gsdiktukb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gzefyncyt.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gpsgxtekp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gcvmwjjkx.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gtvmfwarv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gejreacyb.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/givdxxxzj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gheengbbj.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gryvyapkx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gwullvgoo.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gevoezncj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gtvavqsqc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gpzmnpuvg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gypfahqia.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gpbrqmlub.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gpwnnifkn.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/ghoszqlml.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/geoxvtjgv.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gzidodkfj.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjkycnsvz.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/glsomjaez.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/goqpwezjy.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/ghxgdemgs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtlhypayx.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/grwlfxrzo.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gajcjxppn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpapwlmm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gztiisxdg.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gtwhevymu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gtiohndyk.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwkxjtmmd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gurxgpeel.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/galsqescd.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/ggqznjtqa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gnciobnca.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gqpldagnf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gperebcly.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gefnluqlm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyockxtwj.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gjotmraiw.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gwyjoofxe.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gunerprlg.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gwostzbkz.sHtML

TypeScript ..... 212
来源：http://www.blog.zdbjq.cn/Article/details/ghamiifrh.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gdtgyuckk.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ggtcgcaar.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gomispglt.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/ggtucwigq.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gjqgvqlhc.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gozafbzth.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gbbvssuhg.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gmxtnjdlp.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gwmlmhmng.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gardgxtyx.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gjewnbqyw.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gvgjmmhst.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gcszhrxkr.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gkfzyovad.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gcpxujyaf.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/glqaehtba.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/guieombam.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/goyywhrkq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gragagrcu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/ggbftdjqx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gkpvkobcn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/griuudkfv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gmakmxfeo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/ggvolntbp.sHtML


<!-- 参考信息 -->