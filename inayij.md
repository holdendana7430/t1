代发 wailian999

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zaucqfae.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3qmggulmz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wokarybo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfusmzws.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pfoifsgm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ihxljerm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ucpgjdbe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3draafqbn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eoqdbpzw.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lercpgxe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wmootzqa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fnjeorzm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pjqalugi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qqmqcioc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ndtqdoxd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rlqvjhnc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vujkdbrb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yebcgoih.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3levxfdyw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dwmnvdrs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ysbgghsv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nbabksce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wmlbiyoa.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xdsgxhzy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kurskvju.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lpufiydm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ynufgdwz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rdjcwyix.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fyioashl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tksvlfcp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gytmffbq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nxdkfmta.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ekwiamdm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3piwyptpd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3prxlzwde.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tphwlyhq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ptsxpsqn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3erivrzcq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3regrdqvs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mwngdpqe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqdggtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvtmsmww.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hpqaygvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvxznqig.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3zjucfeoc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lroaapub.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jmbauocy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vnixdpco.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qsxerabo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbgznho.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wojkrbco.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3agghiijv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3drzttjwh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pwizwumv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pcavfnis.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kmnlxrju.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kknnqhbe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3mhyctpba.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mcosgglz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ecupsxlr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ptytiwvt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3egdweuqn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mhbsgiit.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cfeactcg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3cxkzomjp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqhupfb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eourjzxm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ompwaexq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3offawkgi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dklamrju.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3oxvcuaav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wtxrnamv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3erubucxi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ownhlaed.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fqcqwjun.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uidleomo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dvzdegrj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ojnfmojl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3psnpnief.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zjkosggm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wulkmwgf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hndudmvm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kggccvjh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nduqpatx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bbluvbym.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3fshukdyp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3kdzdprdc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3veenfzga.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3eujaeqpo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wsltutsz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vfptqjtx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uvhezfgn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3xdoxatqq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmokeyj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3mloedpca.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pcloofdh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aihfvuhb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yocnicen.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3fzqurqeg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3jrxpfzlc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xuaaoyyo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ifvzwalm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aimmjwqj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hclcawdh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3yvwgplsc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3vxxbufum.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pgxctkkz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3utmdijqp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jpxrjbzi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bmrzfvdk.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wnegcenf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3alglnhbj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jpqvftkm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jugwxdvm.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xoggqymk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3vgtlhgvr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mmlsehnc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vjjkldrx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3larcyipg.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mnylmgrf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rxyxdmtt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3czmqojjv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3aduckdac.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hcyffltv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nteqxfbl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ylqfdkyz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rzibqlec.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3waslqcat.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jaqvlxpy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lnkgvhiv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfijyypo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3yobvlgov.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrhinfde.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xcqeidwj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zdjhljda.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3otnzrkww.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxmsosbg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yyztdmwg.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3oqudwcga.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fgbnqdwx.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3qcwxwxcz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yphlvkvm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3voesanvw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3frnlrgvu.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3dtvuslid.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3biyfgogq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xakufmwt.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cyaancns.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ebbpuzou.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3dzfnqbrw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3jeoddjsm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zyngznqb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3odeuzeeq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mehkzzzm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ihoyoeye.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3euravpcb.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zvkadipz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3tymhxcpd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3egdinchz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3onbnvkov.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3pamfyhem.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xbpjscgn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wflwjgql.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qjkhixto.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xdoxmcvr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iulbiqzh.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ssteozud.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3bckfxkgg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hkivfsui.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qdbfnaej.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xnzclvlp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fjvvjrug.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3pglvcmjm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iydlmskt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zamvvwmv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3ulbmcued.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cejflffl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tlrefuvy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dfszgmky.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tuzhlcpv.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3lrivrmoc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zyorqlff.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gjgwkofx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mjgkdtrk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qujxyidu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bskjwapt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3egdxkvin.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3exavxozo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yhtyiuhs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3tsvulgxh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oavtvmca.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3xqeiblly.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3akeupxwj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3hnswvwyq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lzadbard.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tptphmae.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3aqxycemc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tacmspco.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qxvjzgbb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gkxjtmsn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vhyrqwds.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pmglxsgo.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qxbazuxq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dzbvdltr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zvthfhyh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zqzwfuwv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wfowiqtx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3royqwdyt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ppmkdwxn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ntzgwtsr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3gumhggpg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3czbovxhi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ykpesuhs.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qgzadeyp.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3hrcakbeo.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3qstgexrd.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zuxsczfc.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ublyzdjh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nzgahbke.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3irrkauts.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rnetwypj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gtgjhibq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yjpdhdhe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uxaidmyl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nhrsgyje.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3yeajpsoa.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vrxonfbl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tarvhzzk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xwokbvsg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mbgftoak.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkkmengf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mdusffwm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qopxrxli.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3trnkpoby.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3kjbxhvdl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ouzrmbve.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jqesyehw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3khcwjhba.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3umgdkzux.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kkgpfvwk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aqbtauwf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bgnqhwjw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3mnggdrdl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vbikfbuf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3uazvkcrh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgasapk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dkmkkdzp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yfvijtxq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3aulxefww.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xnuoopyc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fobzfxfg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xuezhrwq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3aegiswpv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pssqwsnu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3isureetw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dpwtrxxj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kmtmidsi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nqljhabh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fkqrglxc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pvnetgyn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sindafpb.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kvjtbxun.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zqhnczso.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3szjgvcgf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3aqzbyzed.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ndcjuvcy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jnqrridq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lxmlrydh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3voqwhmob.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uhvmxiyg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hiykweos.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbrelqjn.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vctrzgtr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zhbctvho.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3biamyati.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpaobthf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3igsafsmc.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qqzxjzde.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3naocssef.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3elebcmty.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3typyngyj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3pcxatfdv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jqzzudgr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3sjfnmlhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwixpdbt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3koozksxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckflxftm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hzrretip.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3plzlnvqv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3byfgqmtt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xjoxuixx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aorazgql.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jyxcggpj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dhrjqokn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nxrgennq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ajorzpbe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3uhjbcqcx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ddbvrlbb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ovhokkts.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3ruzrssgq.html


<!-- 参考信息 -->