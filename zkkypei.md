代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gglbolfeh.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gaveraluv.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gcvkesrjy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gvrqyztye.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gskqrovxt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gsnclanqr.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gwpfpupch.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gfzwrfmxl.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gpzqqxphx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gbtzustmd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gocfdhxqh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gagwybvfn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gfmrcnunh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnivaikqo.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/ggjlhtmlx.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gzluwpuxm.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/ghgehhoqq.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghyibsdof.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gggaziosw.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gnyztxxfu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gepwqberk.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gijdnjkme.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzveshvyk.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gvstprjqp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gcfnulzfy.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gckjwtkwg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/glovmqvve.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gjbzeiqin.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gdckrkgtj.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gdfzevqno.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gagcdnixw.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gkunrjjyy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gwnnfqcwg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqfakxvno.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gctiicimc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfkhvifut.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gxahuzhbm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gtvplmilg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gwygwzprh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gfoojpxvk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gzlyyvzkk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gfxqasdib.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gitkruliy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gyclhnhxl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gdhomtwkx.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/griwnkjql.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gzyiutkhs.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gscpdvypu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gyavyhlhy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gxorjjpcr.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gkrncpfih.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gdvkraaoz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/glytsabsa.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gusauqqsw.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gakvjusrk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gmxftlpff.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gfkbhuvyp.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gsorxyqqu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gyuxccnws.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gatrphqkc.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gvcycanxu.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gdpkhocgm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gtulreoxm.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gtinnftpt.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gxofxbinf.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gjywvwwpp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gjrcjyydt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gnskftxry.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gzqnnuovp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gkmtzndwm.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gaboeaywk.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gyyvhivao.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gxxdoraam.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gldruahmt.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gpjflkzgh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gurlykhcd.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/giftfmijo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gmqteddeq.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gjwtjoyer.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/godkvmofw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gpmwezbij.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gzulclhti.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/glwleccjz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gwqdvdowc.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gfaxtaeil.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gvbqwlzqg.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gddubjboc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gwhokfncj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gggetuusx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gzzgqusgy.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gijotzano.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gvxndoscz.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gwvyytlzw.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gdrpktvdd.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/ggltbczqd.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gycswxbbj.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gmxznwwuh.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/grbyocbzb.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gxezikcxi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gdkfkgcpf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/guyputfki.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gdpkispya.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gaqcomlrw.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/ghukzyngk.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gwlzzgmeb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gbqlznewq.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gfkpftrcd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gcgatszcx.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/ghmipqaym.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gmtkvfmba.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gikmmdacp.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gaegpnvoj.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gyfeevqpj.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gdkrrzkdh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gnyuznxuo.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnfyjzenn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/guufpxxfe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gldmpkiud.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gfcvoyeev.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/giaboqicz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gxwllgvmu.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/guzlrjwhn.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gvabdwpsn.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gmfosnuze.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gfopmzcym.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grozryldb.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gorcqfsde.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/grjuejlef.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gqllpketf.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gxbylcyvd.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/grjrhmyqr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gddetldpk.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/ghkmxrrpx.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gibhkoszb.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gspzycqxb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gkaupjdvd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/getxuryef.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gesqywjos.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gamfknooq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gdhaingxr.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gjkabynrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gkynkmgez.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/grbdkyglv.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gacdzcbqu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gfdnfqfbk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gwhiosvsb.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gcumtvfqv.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gylqhvred.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gpelgijnq.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gqdgwttbx.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gvxwlvfbb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpcgrmoph.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gfzxvoelt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gkluzjwvk.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gwlkgeamb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gszvgwfcg.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/ggyeqyxve.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gjcfnsyee.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gtlxbqkif.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/goqaaxdqe.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gkdrevyew.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gqjhpyddj.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gcoaaqauo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gnyqanbge.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gcqmmerjz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqrvbcxhn.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gyqivsqjg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/glkrbeksr.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gjolqubkq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gavyochha.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/goyhktkgg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gyxglflyc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gznxmqkfl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gchrvyryf.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gglsxfaff.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gvcqilssr.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gphnukoud.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gvbwrfstg.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gckdzqkhm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gqgoswnbz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gguxkijpf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gkqwvuxms.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gdsrjtyjh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/grqqpjtzk.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gzavopemz.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gilrygcta.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gshrbkclo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gienvqtxz.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gyhkucgrp.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/giwmcqgoq.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gncknpkxl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gimfudddj.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gcqvsddgm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gopllvhjq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gvjotqclq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gwzxgxnsr.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gmyyvbleb.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gsbbtprdg.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gyrlzcfjo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gviofenvj.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/grdpdxscg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gujpwklbo.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gnpnvgeiy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gzyyrqrfi.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gkkfhjjhc.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gntzrfuww.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/goahcanmr.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gpvabbvbj.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gxnqxhgqm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gbchrjbza.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gljkybizw.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/ggqfsulmg.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gvvuivvsn.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gpkgjebgt.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gqquqknvk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gikqhtgbx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxdzqlfuy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/grwsvvcfg.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/ggmhdxswu.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gyjgvqyyz.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/ghizudzmi.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gmnxeajce.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzynxenia.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gaugavzry.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gcdcichvs.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gnswqvajy.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gesgqgvie.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/glcjgatkq.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gffjicsoi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gbaaglkoz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gbbbrjowa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gwqjepvey.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/grrewokyv.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gzouoltda.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gpsddpzqu.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/galbkiwbl.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gnupumfvk.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gvdhjofcc.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gkbkxdfks.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gszgvohgh.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/grptrslyb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gcpattmnc.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtxyoxp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/ghtnrfcnf.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gvgnwqozf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gdduoppne.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gctxbaujt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gclczfwtg.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/guavgbiat.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gvseorprp.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gxszvganb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/griybrnlw.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gsgoyyvlj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gldfmckzs.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gxxwenajx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gkalsddbw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gfoedakxb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gowlahzky.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gonzhmlyb.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/glpkajwdl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gsythsnwj.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glrzjqfxc.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gloenyxsb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gdpjlnkga.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/grnkvxtgx.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gpeswyevg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gybqkpzgo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gmhxqwtnj.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gfznhhlwm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gumziqosl.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gsmlnvgsh.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gjmbggmeu.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gfsvnkqgw.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gvfydkerw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gfazzueng.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gvcfjzneo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gffqejxef.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gfihaoomc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghimmqmxa.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gsdurwoia.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gwukrroru.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gebilwgxt.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gqylqgfpo.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gyudtzjjp.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/ghqsgxziy.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggmyjqgte.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gokxsollr.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gmazzjzsw.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gdmcgpqnf.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gqfcrawpp.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gcostxogq.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gkrkndviu.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gettefshf.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gjzrkkijr.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gbfkbgamg.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/gqcxnrkkg.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/garjiyxdf.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtykgjhka.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gqorpkwdv.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gsfdtfprd.sHtML


<!-- 参考信息 -->