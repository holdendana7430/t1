代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rflgivro.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qvsallhx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qdjxjleg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3echhivdg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iyvrrcaa.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yeexucze.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iwxrzfsw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3inrsyrob.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yieqawoa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rxeeabia.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kfdfdkcj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrebzbjg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3shhwcqwd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3njbrkurl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kuxofgxy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3cbqhzdvs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wudwnqkr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddnjxdvq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kdubpplt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mesjyaix.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3svjcvmio.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3inelfgho.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3douetmlr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mxyfcqaa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3evslzkkg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ksjnngde.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xbspwjns.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jathkixg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fptairto.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ewmokjwx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lyttmzwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3clwuagzs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3idpspzdz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mbsylbap.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpiufmqj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kbkstrwn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3smariily.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tfxpddhz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gedamvtp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wpcygxxr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3baazbojv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3myopgnll.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ufeldwzm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vobbtxqj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nvuqdneb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zupxdbaj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmzhhgjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzzrbpvw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3eoqberoz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3brsgzlje.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3tecoysek.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yfibpbsv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ecifctwt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ieapbxxi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sopcmugn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mlrwwmqy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3aophkuqe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujjvvgdu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3czapbslh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xezfggnp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3flwfedpw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3pzegacfv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rvkgfhby.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ckukjogi.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rkqfmqjd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3biyenqkf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ttuodycb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fwecchyj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3klhlmtcs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qxaqqxjw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3idbslkoe.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjczwyby.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ckqqirsu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ztcepuvp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkcpialb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lrrtcflh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lecejytd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3mxwoeotr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hoclclvz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wrqxalfc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3pemrfoie.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3thcwfsox.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3vflxkvzs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hqzdqsiw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3lpjeoqcu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bxdhjxzh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3pbwbvinc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvayzdo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jlgwjpnk.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dtwglegu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3udifuweo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3yhetfink.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vllkxeco.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ibpntjfh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ggsmfkvl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnirsav.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3vubqrblm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iohrfqqp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3sminqwpo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwvgqkg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ryycxsoz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3xfhhywma.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xtwkjcux.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bgtioyiu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3algskgrg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eviqrgkg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3cuwufhvx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3yurqghqs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vfryxmfy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ecnqskyv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ywpssthq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3uwpctdrx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sgmmsvfx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qcabohir.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3snhhrxgc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zquxucfz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3zhgopbuq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3suszwtuq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3yixzcrhu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3sefxcrzg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3wrlotsef.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3unvxnvfp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mfdludwb.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3adijzotd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jjoajzno.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3brsqchbi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wgncllpc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjjqyyi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3eifdwklx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ittjndap.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jwfyslrf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zflzjtar.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iwrfkhkh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3sogxubby.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3oeeonydr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qtttufwg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3dqgbsihx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqpxrloo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mrygrnhg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ajfrswxg.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3krtztjrb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qssxhyko.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3fcmrighw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slckqzrs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kazjeudg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zcxdlmmd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ixrdmkwv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jewmjnvr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bmgxzglh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ufnctuvz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jbvdobve.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3jieejliq.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hcqqdual.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3onzzsxnz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cafeflnn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3irgkkbdu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dgattztm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kjvqvame.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvsvizrg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpzojkwf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jqtutgaf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3kqzwcmgl.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dapgwhkc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mcxozrfr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uuftmzrl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3srlpbdqo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xzwkzvqo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3duzwvmdu.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3sovgrcfs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3krbenqdw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cqgwuywk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qplcszcp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nnshpvfh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3mkthlomf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skvwwmgi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3smtatdvz.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nzexuvji.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lkhfjzdv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xhcurnsm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3zfeucruy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fcezvhmv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mafcglxk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3miuccwgo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ycuszhak.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3efpujqni.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3walovoux.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nrlgxaye.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3oknfmssh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eziibvwf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3okibulmh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3zjvyuppx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3chkfyemv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qorfhdpf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ukapoabe.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ridbscva.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xqolnhrn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3urkurbke.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ywywfgzq.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xtfutpbu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ykwrlmlq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3filhzlkc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xaxtznnd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xvwufejv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qderieup.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ukwfpqxx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ekgcjqgt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rwplfxin.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3drofpgoh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fyydkuwr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3yuluflrn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3qmiysgsk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3knxcrpwx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3lccgrzro.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3viwvjmmq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3wphqwtvv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gkshdasy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3gqddmidd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xbvcejcd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3kmhnllhq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zznslexe.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zbywtldt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rbwuoojs.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3kdmanqdu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vnawimci.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jvuegjsw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gducgmga.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywqlbgyt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zttcuekh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3znycgzys.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ngtromnd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qsthfefe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dluhnflq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bwgdnhbq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3oxtpgovr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dyrlqaoo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ulovtgnc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hcwhtrta.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3eaxgkcyn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3snhqnzbh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmvhgffn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3edofexsr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nkrdvolu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ntyvqfpl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3vbitpaer.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tnjteogj.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3looddxcs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tnmkwsvx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xgusxsgq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mwityozs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iyqrizti.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qkeoxmrx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bjdopnch.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3vjyvtpst.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uuclevbd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kojutofz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yxemvjyk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ghpnnzzc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ytbfptvs.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3olbdrdbx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3andavgvf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3frlmmtkk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ddojerju.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qowxafch.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bnewofks.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jusvctnx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3oizetwsv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3cyalnktl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3wbolbpix.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ujwoiyth.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ruazqopi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3shnoamld.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3epuhfrdi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uyqutnrt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3egshggmt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cmqkfelp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cxarawxq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3eygalhls.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dtgzmqjp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3gldvozkv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjwfwhcq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rcvxymvs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3sxbswyrk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rrdielet.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3scqdhtbl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qkkezncv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rpsfejht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3auzzmwet.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3skuqguil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzfgfdxo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mgaigqiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhxaugxa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ehiszmpl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3nbfbhmyh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nsaluzwg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ruxbofmm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3blgrpaxi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nxiqximd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3pccbzihc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3htizepst.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3buqigoth.html


<!-- 参考信息 -->