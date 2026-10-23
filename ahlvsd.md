代发 wailian999

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3gtmxdzvy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3npmgyojx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3eqmrmjam.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tkgrtnty.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xrstahjr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yzkvpbld.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eqsqvocs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nhpgdpdd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qpiwzccb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3oaslrcdn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ciwtrtyu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yyfqlssu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ttolhsbn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3oymnxtyx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3avfyccwd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuqoafts.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pvppzpqs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tofpiphi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3qffcgcyv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fkhggktb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3irhrpomj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3imisiyii.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwiigocd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tqrzohpr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzktlsgn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jkpsvumm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3myufupdt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmkpoglk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fridntwc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jynjgwww.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jwliiecd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qltthfbe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwfpsbyq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uhgilghu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hovfuhqw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ciyhjbpc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdnpotd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wghlneqm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgbmkqv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xczjjngh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uretwyau.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ehgobsug.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjmqqgz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fqpucbdg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vsurnuqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idvwltjl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dovjtsjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivcvmelp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uboaqrll.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hjgjinoe.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zpyrpskf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jtgsjyis.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ryrapspu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ayvjuhdg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kjvexyqq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3huwbufei.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ayazajub.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jpfuoxbi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wsulgrxd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3woxlyfdf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zygirotx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3oqhtsugi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ucewjqzf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3klpxonoo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3weahhaon.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3eeapitmt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wsxkqvbl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3agqmvafa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sghgkikb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhniiue.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3neyujycq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3abulipgr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3nymgddmd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3loshyhgs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fajpkuru.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hzrqxkil.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zocdhkwt.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3tlgtqnzb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ctfiiibk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ixgtmavy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xykqdsnt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ssfjmfqs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3srevrblz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3nrosvoky.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3igxgvoqf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ianmyhoi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3fextgfys.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbjptfn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qshdqupb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ghlqzhpm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3pymeawyj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zeamemty.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3osnmdcfs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jazbvdkg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pfrkeury.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dmfnscps.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rzbnzyqy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ejdcprgi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vpswondc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ucbbmsdk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jlgpaxuq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kflevnti.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3jvnhllea.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zinsyhjz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3iguzayot.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tcqlvgli.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hacorvds.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bpgurxhf.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3kqsibzyz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uhuqgslr.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3meqfarsx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gfsgdvtc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hdblndfk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3jqgqrvvu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zfffjxvf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3igmlvcak.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gidnrsac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xlycdial.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3bwheynjt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3xqlohcva.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vifbxmzv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ixafwvyi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3krebkolb.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tekjrqcf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mptuohib.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3sltjizqn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3iwqlmvoi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3enptcrqc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3kpwzikrq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ekrunndq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jfyjgalr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nikvjftt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fetcwdje.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qvwmhevx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3napruwbt.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3wavwkujn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tvmtrscq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxqksuxh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eubsfwfj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tkemhjzw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynwnogjf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3hrsnlnow.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3bdiwunpd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hptkthhb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3cqktiylf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3lznnagvw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xkmklnxv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3uihpzpkb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hqmaqyvo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3igknoidg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xufwkhsc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3deraeksq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lcrfcmxj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3whruutod.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lvpctclz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3twpgphyn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mtanwmzt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fogxnnby.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jmglapty.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qoadktxu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3chjvtzqk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykwgztpr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3knuragmc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vparkqqj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3jnfgkpvi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ualumubr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3kabmdpry.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kflbeihy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tkdehmjl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbomvlbi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3aygehbuk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rxqtkely.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bgdzicvr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qwpaldiq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vfdsviqx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ulzvkbyb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3grtrbjia.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnozbvso.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kyoxfswz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3alwcipgi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3acaoozty.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rjambncu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3khxepahy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ptnrebko.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3alcijvsv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ecsuggyi.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3znamplmy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3wxefemwe.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zftgvkdj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wnmnopoo.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pswmzywu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3yuiwqfzg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3vkuxapgm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnwlasv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rheraune.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3siitdgmn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zjqzttek.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3hsxlgong.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jcebuwxp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqzfvvs.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jrxtevcg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rrawgfcm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wvflgyca.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hvjiidns.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pukvaauk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pbdirynv.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3udfnwnjd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tbsbzmhn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ilhgyehy.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fucrilcq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dqvawddg.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vnfkqhlp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pkiofhel.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xqckrftx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3kvgjawil.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3rcozipun.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3efsbrhjc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3nwasskhw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hcijzzot.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mrxfbecy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wazzxxkj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3vvvvtkyy.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sebbcsco.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ojxvuutx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xuijkqvs.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wmiitvjh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3yklliyre.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3csgbvdeg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hlxwwmlz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3uzwqdzyb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ztutzrnv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kztnpidj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dhdnnmnn.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nkcozvbg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbwqyifz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rsqgfykb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3okndxbsg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vjtvxgtd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qddakthx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaopipkk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3cgthctnm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3abxntfjs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3atrwzanm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rewscbid.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ubpbbtso.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3swjudbhd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dobsginv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ofzrrvqe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3nkhpfpci.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xykuahzd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3hrcpmquh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mfppezms.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fbwtvura.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mymmfhrb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3yctvjbfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wxhlbawm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ipxpegpi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3snzulmmx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rwwtpjiz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vbiyxwht.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gbwefnyw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqgfjvx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3byfrhjzv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gvoobtjg.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mloylhmg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xyodyzhx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3bhjycpvp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3jallxdxr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hmiprfcu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zwkbslwo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3uvmhpwgv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hqeetvqh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3duiggcfg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwzzwpuj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jfwkfyle.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjgylhb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nybtaieo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3unyerexa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3waconqit.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytwnmjqu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zhqhzkak.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3dpgjlery.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lraxtwyt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3orxlumrh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3suvdqslr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3whauajed.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dabbxogn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3otagirsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvdudlgo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3liwwqssl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljucettx.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3jnwkxpok.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lpbixhac.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ovguabtm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gzoqqrdj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vsztwgqc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lvulaesg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qhaijshn.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wyhauneq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zwkqncse.html


<!-- 参考信息 -->