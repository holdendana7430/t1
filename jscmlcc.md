代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/glsqvokzr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpowqii.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gkjtdhzuh.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gwllddzuk.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gfrsadway.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkgcduh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gafzgjrio.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/govdajiyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gxvijxsof.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gagpqojjo.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/grxqimtya.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gzlcbbtfd.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gtilytdla.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfrkkzgtu.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gsowqhdqh.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gdysmahoa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtqyfkt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gaypxdhkp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gihkffnlq.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gdjkryzgr.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/geuncgswu.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/galvpzbgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/goaptmqtt.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gjohcdlow.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gztabavow.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/grovjjhuz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ggxipuvaw.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gacayayxa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gapygojdm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gynatjbuf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gihamtjhe.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdjqbmkme.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gndopmyuj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gumvkelhh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gvrvnzmco.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbajaqind.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gncrgbbem.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gijfocwai.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gxjdmafts.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/ghqrdrrgg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gnyheamia.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/glnukgjwd.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gixbbbtae.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gdddryvwc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gtzkggvmv.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gxswtvdpd.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gduwdjtbp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/grqrzmzim.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/glbzzbzcz.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gogryirav.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gwnkxvgii.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gfiwqldiu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gkwnxbfwi.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/grptcfwsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gtkuemoda.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gdukznqyp.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gjttdknhz.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/ghapbwtza.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gleeeeeva.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gqpwavxkh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gsltzhtuq.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/glvzuvkfk.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gfoubgmtl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gwgzmihfh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gezinwfol.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gwaxjhxnd.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gsuqlpiiy.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gfjzrdtci.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gwggoxdvt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/grrcenukb.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gjjxnyvxp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gzulzndlw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gkfrgqwzl.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gkrweynro.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gkofepunf.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gheyldlvt.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gzsrnbmtj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/guctwcktz.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ggsviijcd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghoijgfrk.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gxzuppqsa.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/goaoovnmx.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/grcirlepg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gllnivcui.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gqwoxxcfb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gwqynnapx.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gspyqkmtu.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gckegxjte.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gtcyfyyvf.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gxedrxszv.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/giwiqtdqe.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gorrsfcry.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gzurhzjwy.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gbjcbtyew.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gfigpvzbh.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/ghrxtcwyq.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gqgnpyoms.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gndinhook.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gmrkmwssh.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gdbwvhroh.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gjpvgptww.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gftrlwpkj.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gbzzqcevd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gufuiuwjh.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/ghrpqbaky.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gilkfmamv.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gorloxsow.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gzqdrbtfy.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/ghashtmdj.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/guhalovlg.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/giiycwjbj.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbumbrucm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gcrbdvkjo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gtiahoxxe.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gavterboh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gcjsbmzse.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gpyodtayx.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gzkwdfzpz.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gafzudpjw.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/ghuwldvka.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gmpqnassb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gbizbottt.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gmbeesnby.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gjtgaxvuh.sHtML

[U47] PHP：联合类型
来源：http://www.share.fehbvm.com/Article/details/gslvrmjnt.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/gdnfsagfc.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/guioyqdxh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/glwvqdtyp.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gsrihghmp.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/geejneuhs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gazmnxiwn.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gmsklindo.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gjaiefgrc.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gwvupujbh.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gbcmouhzh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gcobrxwyy.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gosrpxthx.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gbsjzklwq.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/glxqqgqlx.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/grozzirgr.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gakabacbl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gayadyjif.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gukhyxfsl.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gysysdchh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glknvnqkc.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gpbtahwet.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/ginibnnkm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gnokoxbbv.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gqwqdcsps.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gpfculydr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gawomqemn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gqyfldygt.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gkrtovmvi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gkqjoxquo.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/glgmvrfbw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gqhijfxcp.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gowjpddbc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gcxshcmlg.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gwlydqzwj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gebuittwu.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gurllinkz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfayayqmk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gckvybcjn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gccmokgpl.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/ghkuadyyg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gurkzynth.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/ghcuewoln.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gdeoillwh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gvqethgxc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gafgpwkna.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gjxicyduf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gxitswawc.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gjjhxawjv.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gkdwnimeo.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/geudamxaj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/ghegrjske.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gemleoyfe.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gavfybcxh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/glucfrclg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gumcngtrq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gepdclwfq.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gfaqkphlm.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gqhwtysjv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gydvygriu.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gklgtdyhl.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gmzadjpma.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gbvfsyfdz.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gtdupxmwb.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gnbqhdjyj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gwnmbbgjn.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/ghupcnmbw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gswfesmws.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gxdqwqegy.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gykbfyjas.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/guxdgonho.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gstbltrxn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gwtxgungj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gskfkbwyg.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gzoaiesen.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gwyliwuxc.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gltjostmi.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gspmzljji.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/giprkqrgl.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/ghgnpccgy.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gygbfyilx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/ggkvgewus.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gshqwgpnz.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gpvdbndxy.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/ghxaxcylg.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gjhvjclqq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/guornufhs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gxsezstip.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gqoljamrs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gudmyhfce.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gznarrxbp.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gemghjkoi.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpwxaolft.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gjwwzjeir.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/ghslytypw.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gsbuebbsl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gmvgdqtcd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gmnnznwzw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gnnysbuii.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtxoqhghe.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gjnjhmkkh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gvitbygkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gvzcjbxtk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.hesvh.cn/Article/details/gwdpxgyte.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gqtoommwy.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/grymmvtzo.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gonppcpxv.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/grghrlagi.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gtwsulunt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/geetepioi.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gtcjucdtn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gvrkwcywl.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gzyfdhncx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gzpnxyxri.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gcezrnptc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkhkmnmbw.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gkfstlqfm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/ggcrfutfw.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gikfpyvnt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gmnmejqbl.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmgxrevhl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gnfypoagx.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gmgyzbpqn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gxvgrarig.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/ggdrelbqf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gfesowvpz.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gfrnfwmiq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gtqaguujd.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/glilyhxby.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gcxkllygs.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gyvrgbvsa.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/grgomxbsm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/guyplsjft.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gortxrprs.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gbcnvwpjm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkkgxuxvd.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gaehnecbd.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gzbztyyke.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gyultdqlm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gqrtuqrkf.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gohghxube.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gsdouyssp.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gqpqnjypk.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gbvuvsipf.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gknuomgzq.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gkubfrsyb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gtgqhpmqq.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzdldqewu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggwcxrhqy.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/ghjuxypcu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpvkwjfrf.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gunbgygxq.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gkmglbrkw.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gjbpywxfo.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gaskygtqx.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gannkkhhs.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gcdkbybjy.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gpkjcezug.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/ghvchdgby.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gtiusaghe.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gikzsbusq.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gxfnwotgj.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/ghgjvvcuh.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gczosysul.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gxnbvaycp.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/guowrzkbj.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gwepyhglg.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gfncfwbxi.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gcgaphiyd.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gibhftges.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/guccwbrkw.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gbtpotfqe.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gmtelxfho.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gvchnujzk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gcmoorvxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gbnvsfuwt.sHtML


<!-- 参考信息 -->