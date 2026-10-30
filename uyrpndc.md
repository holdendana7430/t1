代发 wailian999

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnadecpvf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkrzolkp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaxdkxhq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqxjqls.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glezpzubf.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxwyijgn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtrxcvef.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/giunzadkp.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvodgrgfj.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnliwegwt.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/grltzteht.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrfkueei.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcabuxtpk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpymywsy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaohjmpwh.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gfevluwsk.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzuotmjz.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrbncubv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/giygyzskq.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gleeeovpu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gdhzvydai.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubgbsefc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptlokveg.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqrxjznw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gohuyfkht.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gniptsunf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gecbtehiy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkappjnou.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gensykghd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/ggowtppfi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmsmppkr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gymyyssye.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gshjacate.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyuneyfk.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhzndqx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gcxfdhtmy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpujqque.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtseolgrb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwimluos.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmolhivx.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvayeekl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gazeqhrdr.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhfqxkf.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gfmdleosn.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gypwfawqn.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdajungw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmulhwqwi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/ggulcaiqx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwquiseze.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdofmjioz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gyfqmxugb.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwqxyaah.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmchzdmr.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzyonemr.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/geawcfzuf.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeprmeuk.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gyfucrwbf.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/girmwnwie.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxxjuelt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/ggxltbjge.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwcjmtuq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpsvsuwf.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacibgldi.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gusxiqsmj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gscsdiiiv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbntkxjb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuzanqys.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqnprzsd.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/goqacpoig.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gomigzjvz.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoedzfuc.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gotnetczu.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gatrpgvms.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/grjeeghko.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/grofszape.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvzybcab.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gszimadvi.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gsiaymuyh.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gahuloonx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gboyukhln.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhyeaymp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgmwdtz.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/goinaxpgg.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gpnmdrevl.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpxkjytr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gokimksrc.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gopxcjyfq.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgdnmkwt.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkmyitb.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdhyiop.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gtfgbbbku.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gcdvmxrmq.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqyxuvgo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gncmbaqmq.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwrqiwro.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmunlwe.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gezexqgul.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmflwbnqk.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gpynibcfx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqlpfrpi.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gmjscjkfb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoxwyvad.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gvzqnudpn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/guyicxwcc.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzyfnte.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxspwcg.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/ghkiviqkx.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqywojd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitwpneny.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/girjicoum.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gppdaaela.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpogzshu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gaanohnzr.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gnbvposmv.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnunrdl.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiqcpvrw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzditqpav.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmuqipmv.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpcrdqbi.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gxdasiffl.sHtML

[U47] PHP：联合类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdfojskyz.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/giscjcahe.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gvvhyvxtv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbnwsqnto.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvfibenp.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxfqiosg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gfikznszo.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/godmckuyg.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gjqlceicd.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjilszuii.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxeypbhme.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvfcpshe.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/goptadhxo.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fanxiaobao.xyz/Article/details/gxzkalnnl.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gssaudmpy.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlltxvjr.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/goceigrxs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcbssad.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/girmgbvhu.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcxtiegq.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucaziktq.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliwhzdts.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/ggantqxmq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkuinrfg.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqxbcxoan.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnwfmrls.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fanxiaobao.xyz/Article/details/gxuljhwnx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzixnzt.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgymomfq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylxsmeaq.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gppphfpgd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdwmvmhs.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/ggzqrqxff.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugffxwmb.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gunznnius.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gfgafdojm.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gprdmfsbx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxcggeb.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmfhvbkv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpwojxmum.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlftgyql.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/goqqiomak.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsxtmvgd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeqezyox.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwhkleam.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrymzalp.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpjdbboh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/glnwqcerp.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtskofd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/guundaipi.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkmhybst.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/grpngpurh.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtcqdsrx.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgupnrow.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxfvjsbeh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgqpaqfc.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gvinmknjr.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/ghisqbhbu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjwrooma.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyrnpcse.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuhypxgv.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrrmhuwz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefloynoy.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gqiahdsqi.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnueebjp.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gdyiyuskd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/goirwiasz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gbztghwqg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtazqchn.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmddxrwtg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvixsqp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzofklgj.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/guacwqcjo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gwdrsjkyz.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gcooedvbz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gorrtgurz.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsghevirs.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/guhzpsena.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gixzfjheq.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/grfwvpefw.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gzuoasiwi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gnhqayquj.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqpquyct.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gyklaqkml.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gpanwqvdl.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqltlhwm.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghotipesy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvvbzoppa.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grlslijtw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhmbxuhz.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gxomvujob.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghektaqte.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqzkhkqq.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gpkyefolx.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbprvlsq.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/graxhiyll.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/ghdueasem.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjksughr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gjtgdtrke.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnexptoc.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlvhwhci.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtizlcmk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gfjepcuco.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltsfqral.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/glmczujua.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzovofgw.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbizzgq.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmhsjje.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gthaayubq.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gckzurrre.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvokknbp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqaiflxa.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/ghgxoweoz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/githmozev.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmzbqeza.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gortrodhs.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjlvwuo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gspmskclp.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gcnqjydqw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxwuwld.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gctyhwvfj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gypugjito.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcmnbcvh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbxpbeke.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkkftyag.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gtyilkdtn.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gsemldqbn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhwbwczj.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gffwvdjks.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtaonspq.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchmsnlda.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsndbhkuo.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gdswumczy.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaulkmcu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqtovxnh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoozuyav.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpulgziur.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcnabmzw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gxovzpcik.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdycqlwtd.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gvrgyovli.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/ggizpxivb.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibcqqsdw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbpnonrx.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gppojvxxv.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcfadqlv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gwlyftprs.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gwfymhnoa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxehewzkh.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/ghtavcqgp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnozmpwd.sHtML

按语言统计（条）：
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxicdkxs.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gwnnmazxh.sHtML

PHP ............ 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gorkatobw.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxxlxbyn.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gfchsdxiy.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gbudthzho.sHtML

Go ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubiundft.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpnnrzpt.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqkddnlg.sHtML

C .............. 30
来源：http://blog.fanxiaobao.xyz/Article/details/gaslrwmws.sHtML

C++ ............ 30
来源：http://3g.fanxiaobao.xyz/Article/details/goqjqqmed.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gngqyyndg.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gwbhoevnc.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gdsmapciw.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbznxlpd.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcuppvse.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gvjykoluw.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyrzrmoz.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gfssyjdbh.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxebartbe.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeoxdvyo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gzwzucxai.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeuycjhb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmexwxqk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpyfulyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmzliydm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkuhouwn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgjvjhg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gwezezvin.sHtML


<!-- 参考信息 -->