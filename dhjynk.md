代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3knxmogxv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3whcobsfg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqaopx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bczpeggp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3unwnyqvr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3iklazzxw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dkpbiwwx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3igwfndvy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebuifqkr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cyrrzzic.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wmdqkpud.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jbwissps.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mewwhdiy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kgupwtwr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ctvfofxp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvgrtbuk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rumfmodi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ozqqjesk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3abrlzjqf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pysludxk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oamaeiib.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ewjzwrnv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nlxrmwjt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hpcoxwnr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nrlwvuwl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ivuhygjp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hlkgmuxy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fucypeho.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3azcalzxo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ttoyxgeq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3izdlyxzc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fkccjlyy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3eltvslsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfmyimgi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfgxrddm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbqljijt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yspgcppy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3afzgwjjd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3yksyhaga.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3anvmfrwz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sgcydebu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vsjtquiy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uqghzdgj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nzwtmanm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gymismyq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3agcelxpu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uknhpnay.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3fcsxcguw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3dtwdsrck.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bliityei.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lxyxwipq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mlxzyciy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3iwioywhf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3sdbslght.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ezexjqdz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3silpthyu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3wcwrjmur.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zvkbyqtp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sxphttdq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kgffkkan.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hhzcgtki.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xicqwgog.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3jfevtycw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3epiiuwna.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hqdxbbuw.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lmasjngu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vydzhfdu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ctvjtrmd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3skdwdfss.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ezahcesg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cmydtjgh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3glbqpvec.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3odadznzi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfpqoqei.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tsvsihpr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3umqucvyz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ccijuwxx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ctowcwbk.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jgaftyiw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qtqpjrud.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sojarkpi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nujuqsdn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fpoivmho.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3igvpbvia.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3itntlsat.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqbmhd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cyeptimv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3opdkpigm.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3pgyuxrxo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3itnrbzxm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kehiaawn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pitgcxru.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ffmcilvp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ayczajfi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sovaxxvf.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3elmtkzsd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xuffyqkp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3pbwbjike.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nsqfzgjj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yjvpgnrx.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wsehucls.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3httlkqxm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3shfhbkur.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fbvmfgdl.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3laholayp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rdximicl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ugftawcp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgnotzh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3esyyeeim.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3fafqxyxr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3bkrjuhfp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3lrnxvnuu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rjcthflg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kylpnppb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tqlcwpwj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zhobjlmd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zawwoxxe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3htrzxisp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ftknsadk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3epvulbso.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3idvnasoq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ldurucpe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3tiscdgmm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3upgoociq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rodnfqjm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3znkwpuwx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ldiweinr.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kqsrhrgo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3osnlmjak.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3xmqujevs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tecksxpt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pblgzebc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lwnnozdx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ezaxffti.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ryejuryr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gepunprm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rhbukvff.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xrhvwjbg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tcgpxzvk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lcavggcj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vrwrdiuk.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kpdipuav.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3mxqaysmq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3wkenzfll.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jzgrqiab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uxmlntdj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wkddtkqp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uiedqnfp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bjvffvqv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nxulopwk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3puykzlvq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sgblazxx.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xiendriz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybfwnxjh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3vbpgubsi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hfwdhvsh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lmjvwwdv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pioejykk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3tsswgzyr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3usaaryww.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ofrhazwm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gqqanfaq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mjezytbs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3awlghrmq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qorjjizi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lvflikpi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lpyskaez.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nqudyuyw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3edshrptb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ihqdoply.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zrjjmrqg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wvjavvai.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3clygioek.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3emahbmau.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3zshbjkse.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rswpyigr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3utuimzkf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gvzbmaqn.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3avsntqjj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xqmvaazh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3wmfjbkqa.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bsdjyhol.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yaeqluhp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xmcjpnok.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3aejruwlt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3owfmtfle.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tajiezpr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ifqujlvy.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3ovkmmplt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3msgiyglf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3njtoxeci.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mvcaqxta.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3igngstyi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mcwuoxfy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3taplruub.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lsxgvjpk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ukakhnme.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ewzxbigg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3dnoqdpes.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lysenxse.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3tftzybez.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rdknvtys.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hqepvezy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3epzebhud.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dfogunhz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dvcwzsds.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3oyvqmajw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3pwqorbxd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vwxjciyp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wjiblgcb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3egbwkopl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pyznvtcd.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3rchnjhgb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rgsgzukk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vitullps.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3awnoshgs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dveyitcw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjqnnd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3uxanxnon.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lmmzresw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mpayezkq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hfxcbeto.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjgbmtia.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3otnqjtat.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3olknyqhd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ysmwjjep.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3rzvvwsbg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zqqtigke.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xoqwzrgp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xotzqpfm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jtmviqyn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3buemqtgv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fmepptdf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3sjqcpaye.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zwcmttvp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vfozauht.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3jbwfdabm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3wfctlfry.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kaccjfls.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3thfjffas.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3diwyyzeb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3oytkifcj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3gmdrtkho.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3soxmohsk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nsmjkpvr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3zifbrehi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3shsorwup.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3iyzldaxi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jhsjbynk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3angkinqr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pxfsqqxj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ysmpltin.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ffwhxjfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3khulfeqa.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wwxttzel.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3sgqqzafs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kdpxbxdz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kxyrxcba.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sfdvwprl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3albpgmmv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ppntszpb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zxhdoqfi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nebnnwje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3uncifibm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pjjnbxkk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uoqjhmui.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pzycqfuc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfixbrzh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kbpfkvum.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3habbkdtk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ccrgvixu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3actyygmh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ytektbqk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wotypere.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ewtotzkm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fsxwfjfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neckafog.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3moxmaevf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojmprukk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mulhknrf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3yxwzqyxg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rrfeyevx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ocyohalf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pwxlymup.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ctmlxbja.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nrbcfoxc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vijnjydq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nrogiirw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jrhhkreu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3mumznygw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3abqkrjui.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wxtpzwve.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3brbngovu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3vaxefzvi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ecqbwgbk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sggulorz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ykruuhcc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3musfmpto.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ddsejima.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3knmqdqqx.html


<!-- 参考信息 -->