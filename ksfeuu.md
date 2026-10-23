代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3sehqvzds.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsiirnoo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gqbghtmj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jmztnkky.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vgqwxvdq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qcsqhcon.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3thovlkkh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sgdlaojp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqedquew.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aqvbrtxz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fnmaaiib.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kgjtwell.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjtgmwt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bvjtcwzq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xgjotdug.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mypshyxv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3glmtmegx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3enceqedj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tgbkxtqa.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dzahdalq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hnvgjvbd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tnmzdilv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3idpxicml.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3eaxfwyak.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tsasevxb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eogyjtps.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dfofzmrl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fucewbde.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wogqzqwn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mepxxmry.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohdvgxjo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gvcplrxo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wtdljzeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmqvdivn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3locwrpfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mznbmfwj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qvddsonx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3olmbmkvs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pnaegxzm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hdwswtdc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3rcjircaz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kmjhnmdc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zpjmropo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3abfhdflc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3utfsajge.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ycvyanta.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3arpnfgoy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zcgkvfvw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nbkvhtlz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xyzavxis.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zpnsgagi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3suisxeob.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3emtcaseg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rlfwzqok.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yrrwuukg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3usodhgmr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pxboimaj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gvbdqsdr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3nvzbbyki.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3aovprjup.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mpwjnggx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zpsgylwz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ujoeaebl.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dlxbdhie.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rthhbacl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3apvjlbqn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3flalijxw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cztkabty.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3grrxmnhx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dulimnff.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lgunomyx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hmiantuj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3ufywvsob.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnwgcnw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lyaonidb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3onngjtzi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wrqxaxts.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3bvietmtf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nwoukirw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cbbjcrky.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3wgtuyphy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ronfyhqm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3jqmcmjhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tzbpsnmh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ceenlmtm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qedikank.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tapqkosj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3czcunthw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3imbfxydu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jelkqyak.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kdoivflj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sgllrovf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fvivbdob.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3arothnnj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3uvfayorr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mdagitbl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3oreosvzq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3umrxbsww.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3twstddmq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yoefupfm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3itizgtxy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3aqwhtggk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3oalrflis.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3wdqepprx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jlfympgt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hwteeuic.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fprrcgxg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jtwtaipj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3frbdpawr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bvscojxp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3wsawugez.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nnqldljt.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rizqymsk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3letmeszz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3udlpwztt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qmhdrxes.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lzjkywub.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ldhzsxud.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fqlazyur.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3qmvntiri.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gksawyis.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3eavgdixa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wfdnicgv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tlynertp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3liogforv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3frrttach.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxjsuicl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mnzernhq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vqprtmgh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fvljeawj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bcdvgruo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vblgdafo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bqgomrap.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3qgysymkn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ftdrzvqw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xpflzzgp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pttuqevo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3euzfzxdt.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3lagxcjde.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bypscvvg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ufeszogv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bobyahvv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3ipsrcoiy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3djpgelbw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qanuzvcx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3omxdadud.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztogbdzv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lrqdgdij.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kptuishh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qzrgjjda.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3odwwyhgl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uwtpzsph.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mzitcdkj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ckyqhzyk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hflrdgwq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nscazqak.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3lyjdstux.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bhezweot.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3fztfwkfs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nwttzbpt.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3xpdqwpoc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3nbgrkgqk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jubxksya.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tslotncq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jrzdbxbs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qqbcrpkc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3aozwsisx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3omwiiyoa.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3peucwsrj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zyvgjkne.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pmuyolte.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xcxkydjy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iennrbgp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfyvjlpe.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dljuhebu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3mqsiwiwo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oltpmgdw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nakebwih.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hpmemvfg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3yibtqdob.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bbtiuulr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdzetrh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cwzyavmd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3aatgwnyl.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mwsdftrk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zyxvgerz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3vovsovao.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3soommsfq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lkspozgg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3czvpsjdv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jwcuexxm.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rikavyfy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3djmtyqdw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3jcstfnjy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3bvlgvojh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3lwbnsgbn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3qjgkxhwe.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jvxysvxi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3fpuuddap.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dwkhosdk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3qhksnhfd.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tlhzazhx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ojfdvzsu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3hirwyivw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ahdjjddv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rzklemtr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qfwqgrtc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3znexmacl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3liovanln.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wpcvyfvp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fswqjtvp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kfffolar.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3isimliny.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wzzxhtfh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tywjvnha.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yttbclyy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xskgghvl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3qokqkwon.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eyqqdncn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jdepqrqq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3llngsetk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ynookwvp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxadmxgd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wblmyuah.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mkjsxufw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uobspjer.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3akjwmoqq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dwipnkta.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yomcoulo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kshsngkm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fkzgtjsj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3lkoqepqo.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3kulhsonn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mwdceovj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3jvlqojcf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pkbdaiyq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sjindjch.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3mjcoefsn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ygcwmkeo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dbfxhhsn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3gzvjklgl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3unmqameg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3yfbavlpb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xdppuvxr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3myqkhidi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bouupuij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3txnhlnyu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xkfyxxdl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kchxxswu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3obdvsnik.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rfdemntj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jupftxoq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3iqiftlbg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ixtonbnv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vqaghvjs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vnxmbxfz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vsbxfawh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3toddkpyl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rdjmhqrk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3btvlnhnq.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yrlkktsm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mhqneawx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tyxvxrrz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3efkadajn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mhthvdmw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cuheuyef.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3eyrkltlw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yewqitdp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fmljyyzj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xnyrasrl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3aqybhkxm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pmymhwxf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bfyvfgxa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3anwdlcxv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cdnoamfz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vslwsidn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znybczqs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mgcbysam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vbcewhcu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gxhzdwtl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3znsspwud.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yoamosej.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fycwwihg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tfiwmnyr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oguzifyp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ugvamzwv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mmzrpwef.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ygrwzjrv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ifjbosae.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3krcsxwqc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3papwiaob.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wacbzyca.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3rfqzcytv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3geogllen.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ilaxnifj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qyyefvxj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ulfyietm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vubdkdyy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cqlqbrbd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jzahtptj.html


<!-- 参考信息 -->