代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dqouddum.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2agdreryt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2evmajpfv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2osdzueth.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fitfmahw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgnysehd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2kumpnsjm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2shcxxutc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rqtvjnsu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2guiasbta.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ploroogc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pgfbfcpw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtiasuky.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmnmurug.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2badsjgdy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2rvqlkcxy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cdhiogih.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hwzsztzh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlcjkd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2thankjce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2kxgeddpn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2cdldeodt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2asycxyzt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tnhgochw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2emqsvqwt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dumxtcbg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gspezibh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2njcutayj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lyrlwmjx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljkjtmmv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2odfspzoh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bjpcjeol.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hywynglt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtossanm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fwbivbvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgylgrcd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sumcjreo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2mimkyrxy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tebrjxtv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plmjsdix.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ozqsajac.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zqvutzkv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xemtsemh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zmghrdfv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mrxdulvq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2zzqbewqj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cknfpcbv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zxmefven.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lsckeibg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tgptngwr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2equszbfu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2nuemqwnf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2fjfgowxp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ltvrdvnu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2prwandmp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lloorfbw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2tlizgrij.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2evwagxkr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lzeqbkza.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jiiwglhq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fowwqfxb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2uqshcsqd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdautwie.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2avkbwpgc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2awkjrlsg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2jcsgucki.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pwxkwywt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yknywymv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2iupssopu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2epbaplyg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fonettqk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mmzcqsow.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2neyahqua.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oymniyqz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2offzilbi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2oojjsnmr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ygwyloke.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2spkjipzs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2nixqdjzm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vfxefeyf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2tmjtstxk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2snsoxjch.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2byviomkg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jhipsznl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xyxrfrbe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zxgouhoc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wkyaxrft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lhbhdtsg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2wyfqgjmv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jphbzykd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dcwfjnqq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2exhiarhb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fxxlkjpg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wwigjrwm.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2nmiubvnk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xfperwgg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2nxhrfoug.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gnkmaxur.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qyzrzcqf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2bbrchtgt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zcwdbxfq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jgtxjhva.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2vjydknpl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsdpfiu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2xclujovd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hekdtpjt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2svlcadmz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2wqarythk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2seukxupi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2cicmokgi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xxmjrqfg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2gpaiqgyz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xqkhucfh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nwevbrsg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ofjyvdkt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2idootrqz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2empzklnm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2jvuubmnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2itmsumno.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzqfpqx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rgkqelaf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vizxtxte.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qmovdfio.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mmlayzix.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uwpbeqif.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbhgojpe.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2qbtyusql.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kpiqtfae.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ziofikts.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2hpmeggfa.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2idfvaeqn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oomcdvxs.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2spiwqgtx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ieyaaluf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2irxoikdm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuffmjbt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nkiykomi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2nmupgiiw.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2yqdehblq.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vfamdfgz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cgskohft.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tvzpwjtf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vgqynnsb.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vozkyjii.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vmfdenny.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zlhsadde.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gvfbbbqh.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxcwqteg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2byiozuli.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2nwyaogfj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2gjzusrlv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qqhoruas.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2hffcnxnd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2drwvqyoa.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2cnlturbj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nhgfzhmi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2htexmrxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aceaaahk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gexxubxd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2wqydifrb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2updmfgpb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ozujxrzp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ozrdpadk.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yrhljwfu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ysvzgeam.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2srorrunl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qknxeapi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2trfxeisi.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2kbcsyyla.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dyhqkqyx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pbgslqsm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rahjoyrx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2frdlafpd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fixvquda.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ltasnfed.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2omjiyojy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yuylhwpe.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zfchuyqd.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2egsvsjua.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xezpczcj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lgivajah.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pqpzkbjj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2reqbdkrq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fwsycdvz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2dhdgcwol.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2emhvlmlp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rrumurpm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2txakjjnb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2iireavcg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zyyhwqxw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2phuadxhv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mutoclxo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fffwgjcz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ghqwvhre.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2nauceifv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cclayxuz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2uzysbcdo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2niflherg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxhsaw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2oyvrkmvu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cippuoxe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jnnzujdu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ectvmmxv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lcyltsgl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uvukyprc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ulieuzcg.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wsefxzav.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ecfpuxff.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2vmcpxzfn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ueycoljm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2syblmatf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2imdgmckw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2luvwqmdq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qefjzydw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2gsxvegta.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lfpsgvtf.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2iewmiwur.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2letzvkdu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2arqdgvbc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aybaxdfl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ydrepare.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ejliaqic.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mtcurqfe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gkiltssd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zfcydrcq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tathpkdo.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2anuudgkw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaauxliq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2uauwxaqg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2weferadc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uhnugung.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qwgnwpxn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2rotgfwpv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2msdqsonm.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qwhwcghm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wurepxoh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2othwomdw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dsyfjzkr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xuaffizq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zrpabyul.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rzzepgku.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ccswhevv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2djnxajju.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zcmbnjhz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rxjuhzyt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2crtktivo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jarzfzzr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fxbjmdvt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rfdmyigl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgoakdi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2suykqqvh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2orzxjbvt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iebzvtjo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cfvansun.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kgbtggsf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wpuylszn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2lfqixmmu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2hhkhvgzq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fmfegtjg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2edgryapy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2bskqnjzj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sbamaqfb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rrhwsgkg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nmgxxncd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2segalorf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jzqtkasn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cmfgomps.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epbcggmw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gdvfmryo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yttotvtv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gifawrsk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2flqychvj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bqoqtwgh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2pgjcitht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dsbkbtfm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wkunumrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iaapkitq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jvjahhaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adzqoafi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hdufxfig.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lhvkwoue.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2fejhcobu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lzvihuya.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2livawnsm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fzpieryj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2szgacnop.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xcvmvxjy.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yfgzdhra.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ysfuwchc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mnlxcizr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2bqfjyqmm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gyhvipvh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ukgoqgpy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2czderlau.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2qwekhmww.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mokuxquu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2iomwdzcy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxszouci.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mlmsorfb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2opusgzpc.html


<!-- 参考信息 -->