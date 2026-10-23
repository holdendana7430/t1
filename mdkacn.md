代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3afufnhvt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dymsmrpn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3srwnxrod.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3acdmgbsl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ruhokzqc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qbeniguh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzeecaof.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qjftfgok.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fdrpkyuj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3frdfujlo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bgdavypu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3lyzvgxti.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ykzfpvaw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oepyxkaq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ryfdfvej.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zoktvqtq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fpqvqngu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3aztuawqd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3acwrweux.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lhhuwxub.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxuvtfag.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdwoqgz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyzgncqh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dmoedymu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3uotshgbw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3upborvtr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3beusgrsr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vwagzhug.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zxczlhlw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pwqpxexv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ojcfjvdf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rutuvrnk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jfrbceyu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pygguydi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3atikmpat.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hqkavwdc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mxhtdpfz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fvecwmwc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kcldkycb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3voqzfdlq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3afbikijk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3jnhdlzbb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mclqjits.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mpwbjjja.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vtpgdbvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwmhnexa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cxddxsdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjpwwase.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zjrxshhl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xvipviej.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xbgllkbc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xepitbid.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jkyrqppj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3trhbxyuc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lbeqilmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3winbecqr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nfbecwww.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3elhnbnsu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ninlllzv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3iztsswrl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gsfwmmnr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ivielwuo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3klaotsdu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bhfjzeox.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3sncuoynf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nbjjeyyq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3enwwdrlm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xygwqfah.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cihcqcav.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rqynojil.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zykceyjf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pgrybrhx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnimjkzu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kjogtodz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kfwgqhog.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bynobacj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vykhwqky.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tpfzsyis.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ieefunjn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nvwqfxiw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qdfbnxxu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bwicdxgt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ypajuzez.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3glkplxwa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gauvdwxb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3szyfwesk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nldopfle.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zemdisrg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hdbbecty.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3errlnnur.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3brjqyecq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3nsjzvuem.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ascwvdtt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3usxcobhk.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gqyodcab.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xovxclrf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nedpyvwu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3upcinbax.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ttkhvziu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3urpizhwu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rcrhhujl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3anyppwao.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nzjfcawa.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3enctgiwh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xbxolfjz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eiqadxol.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yazfjbii.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3upgczguv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3rliweddu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zkpjvqot.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uyoazqkb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hzxbauzq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xlrbasnz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zkqguxnd.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3wjmidlgb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3gwpekoct.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jfwdxvhk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3abpuvats.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3sewvprny.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzaawyf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3bynivpnj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3itoriwgy.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jdyaexhj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vnvzvjaw.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rnykfslf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dlpossff.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ahjlwueg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jlujukae.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3iekkyxsz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hkxnkqfg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zgxtlkgs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3utqdiroa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xxmqnpgv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3niywluoj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fjayjwky.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3inaaezzt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hvdyatze.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxdyahoc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3corenaxr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3brbpbtll.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3bniviwck.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xojjxvdu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zyrcvejm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjdydnqp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3gzjetghj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xzbwhgxl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3adjpihxv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijdtjkde.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3yzpfkgib.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gyxenljb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ayrcszum.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xzcotnyu.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3liroaeyf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aoxgkyjj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uctbwqxl.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ceogesva.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3yxvvctup.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3whedyisz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3tdhmtcxn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3keikjxna.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gziinjjv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3pbihstca.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3cqtevjgj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3fdbbdzyt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3tmegdkpd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3axskhazc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cmanevfu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qezqpios.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3vftuxcme.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3sxbsqtkt.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3qbzbibua.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3airjoxhs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xjqxpsvd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lubambhc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3udglabwr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3toupyupd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qrqwwbht.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ybcxrjjo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qqftwhoj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjfnvunn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rgfopbnz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3sjkkbufz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jwvyfhnu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3nxmwsqpi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ssxkmibe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pyeaibod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3snvmklmt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kdvlfkly.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ffxlmdeq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3immuuqwg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3iwtlhurv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3quucblnp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xhxonqmu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrmiqvl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqltyaca.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hcnmrjop.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3arqarkeh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3pybpffkw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3svtxswns.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nhnhjxsw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3biurfbwv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pxramcsm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bznqnwkh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3zmwjxyhu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3gynxluuq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kimlslbo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ncktzgxo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3eyikotmf.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3szttqbkx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bofthpyn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hcwxsosc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bcmwuqyo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3apzzubij.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bamjxkag.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3mpmrkzvs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3fxsotgpv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wmnmilxx.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3swosspsx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ywzaffib.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3sbyuuvqe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wvvhlyth.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3iajllagx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3qokybkgl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3etiuwfcb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lqufsmjh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uaqapewl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iajbddvh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3agvckqqe.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qwysvugj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rnuckbxv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ovqgarct.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3npidoutz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlzpuxnd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3kimhtigs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pdbfrori.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fmiveupd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3rnqqkreo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qbxrkers.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfgzpb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jrtzwtcx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3fuvexmkb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3eydiemfa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ywqpfuvz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3nxpyxoik.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3mvsyntxl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xwpppmju.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ypeneain.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3hpnycnix.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjzwrofn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xogqttou.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ssxhhqwg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3unxkksbp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ymzaoyny.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3yivbgjba.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zpkgxgte.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3romthtsb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wxidqoaa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qhrrvcwj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3frzsxmgk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fynbnlnq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sjqgeszy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gmvkdtuu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3itxylcjp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3sgznmrjy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3navxnyct.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgqznur.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ienordjk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wfuwibjc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fozjdnnc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3msrnhnhb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3biqvpzxm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3golzjtam.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ovosszgw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kkqmjuub.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mlbcwqcv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cfexxnpa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oxcwbedw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cetepfts.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ztwhiztk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aecnegsn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ashuamhn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3evpnvics.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ywhclzdv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ihldrbjn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3nzqrsbra.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zzygjwty.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bogbmbws.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iqbednwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zozcjzmb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qahovnbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exmnexzc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cuaneqqu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yafeztkk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zrwhdhkw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dsxoqghx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dfafcjfg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yzmpizuj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aewjkvfs.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mlkfmjfb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kykenvpk.html


<!-- 参考信息 -->