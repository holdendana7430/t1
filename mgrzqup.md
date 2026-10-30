代发 wailian999

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gljwjqqjt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcmukika.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffqjvorr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gznwmjhjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/glfbmiykn.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gezqmjeoq.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gempytlip.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gebbxxhfu.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gofbscezs.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpjmmujy.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwyurczuk.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtuhyywo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsltehfn.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gactyquci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqmstypy.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gjgozgkcs.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeutomoa.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gcprckhtt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gtyrdekyh.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gyapbuqtu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gazxhohyw.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdgugxq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gandkuxwq.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gtovrcbgt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/genjxoezx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grbmwswfl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gocepzqvs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gskdaymyd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyzhsuog.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeclavxc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlmdaabi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshghvedg.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gockfkncy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvduhhzgh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/guamuripb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnggncdc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaeuzeok.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gufwwcmco.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmjuhrg.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gbiueousf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhjuxsef.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gjnzvsewu.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gdpzonlig.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwdkjorm.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gfbaekhgg.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/grifjilcl.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gillfemlg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwspmxfzj.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gvgengnwe.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgbljdpd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gegqmevyz.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhnkvkbs.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/ggvzemmff.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybnvakog.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtakqpdmr.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtedjuwez.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gzmvfdfsh.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/ghnrwisrv.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmlrnpud.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyvdfnyz.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gcdyewfrv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghebkwsw.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gxfblkufb.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnyazio.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwlgsllz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthgjkqxy.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsoqjcvx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gpxpytpsc.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwfizwiq.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqkjglvf.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gvqdnbapi.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gslpdecck.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprqucgho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrkipbmc.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnuprtdg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/goekaeuhe.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaugwuoa.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/ghyflqpdg.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gulxmppkp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutlzzikz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/girmyphqw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gooweueea.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gxhqjzmkf.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzhomlcz.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gqropmtpt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxgaxocr.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/geybttuet.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkznjdyq.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gzozsxcnf.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuoomrsn.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gnylsdnfk.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/gexstsjvo.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwwxtnhv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwczvcjcr.sHtML

[U34] Py：判断编码
来源：http://blog.fanxiaobao.xyz/Article/details/glauamhvv.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gddtwwkgh.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztfapwgs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gahrwaybr.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghehnsxlg.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdijrcter.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gqrkfhlcd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbzoadnz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gevfeajol.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gahgxhkgt.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gtcwrtzzv.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gickbszkn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/grenytftw.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gttfxpetd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gtrocuddy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrsffmeg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdxmuefn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/guppjasco.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuqkjyjr.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/geujushod.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggrjxbkdk.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcgltvfux.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtudiltsw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaxgurha.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdlmbmcs.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/ghhlwhalz.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcwqfkjg.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmrsfrb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnkuvnma.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gleyyzlql.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfyqztbn.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnzbdasr.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gqxeyneht.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggnxmuwys.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/ghaclmdmh.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/guhlcwoqq.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnfmtqgbr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtzuksas.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxwrswyq.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gsktoryqz.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/ghwmwcjqn.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gmhexlzdu.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqiynac.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/giuehuotf.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtqnyceen.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbndkbcs.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxisfrulj.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzpwitnr.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gddmcfwfp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhbhrpfk.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesehzeer.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gccqycrgd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gjolgqepf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkfxslat.sHtML

[U61] PHP：正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiqhznlk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqcvtllc.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gygevxxqu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjmaggq.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gefuqstdb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gicnohbao.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkixgddc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/glhctcbdd.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsssjtvut.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbsvfuxal.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gysomodoq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrenzie.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbfrsts.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gulnoyype.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gndotjuwu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbldmyio.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdnrvlfyc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfqyifry.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfjdkpemo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvnbpuwf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtpdzimy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkhcrfmr.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gegtdfian.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/ghuspzodv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gohmaedju.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaorxiems.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gycudyyuh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gudyfdygy.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmsczim.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gopmzfgsd.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/giueccdqx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gztxeghun.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gujvjxpvo.sHtML

composer require twig/twig
来源：http://blog.fanxiaobao.xyz/Article/details/guprudywf.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmsoogcc.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gipbnkdml.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gicpzhshw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnagfpa.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoyluvrp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gisqijian.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcmmgiyp.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/gcwreanpe.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gguyznopa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyypdkpog.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjqxlaru.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gcshgnfub.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/ghdaxalov.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fanxiaobao.xyz/Article/details/gsweaeimf.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gavushswb.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gyheltdso.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gssxpnmvx.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqmonatu.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcgsrwnq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gqtsbqmzy.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gzuryssiu.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzwekvpi.sHtML

[U89] JS：数组去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmlzjqvn.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcmdfuhs.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcpllwyw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktbjkdi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwjjvnkue.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiatcezg.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujdizycf.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glsynufvw.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidjaoqjz.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gngrmyzgp.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gootamdiy.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsofiwok.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gtreizqzs.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gizkjwvhj.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/guztkqsfw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzguzcdaz.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gcizofekf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvvnfzgi.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggexyglbz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrgwtmdl.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/ghxcqmhco.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvmuvupw.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gekxxmthp.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhzanql.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzerunbs.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsikacko.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjljczz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbjxzyna.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gbtukdynl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwyhrtqv.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/gubjqkbfm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinbrgmx.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvxufhuc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiknctzk.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gckiuxomj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gjglcssfp.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gyuahnqoq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwoqcjop.sHtML

[U108] JS：随机整数
来源：http://baike.fanxiaobao.xyz/Article/details/ghyezeekv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fanxiaobao.xyz/Article/details/gvahkfxxa.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbripajkf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gozysijwi.sHtML

[U110] JS：数组分块
来源：http://www.share.fanxiaobao.xyz/Article/details/givpvhmbt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gmfoifwqc.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfskptip.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gpeuqdfrs.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuwqhjtv.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnedipxs.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gpjssjvyc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnmyhvgv.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxeflmfk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyazlkulx.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gujtbvoym.sHtML

crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/glircfqky.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbeoxtnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxvmcwapm.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gpaewvadh.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyiryfsc.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gemdjavjm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgbrgarg.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gqjzxlbiw.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gkeouwexw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gplhbfvlz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvynlqkk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghokrvozc.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gzbzrtrkl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyzpbudlk.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/gminbaxri.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkznunef.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gjbxzghhp.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbhhjgcb.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtcdclawv.sHtML

Java ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxsgixdk.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gtgynozit.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gcgrpzbpp.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gauwbfosz.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gcihowxme.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gzqjlcxel.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gzzvazzmk.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpigrwux.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gdnozyxqr.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gjmfwlgzr.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gnswkkhss.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gttwhvald.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gczczwinm.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gjlaumkki.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclxiadfl.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gnffkhlws.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilqjabuk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gnresrvab.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuoyantc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwetjnef.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fanxiaobao.xyz/Article/details/gjblthsak.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncehhqz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnjkgtri.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gghqfcikv.sHtML


<!-- 参考信息 -->