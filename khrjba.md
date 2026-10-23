代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xiwqsihl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfufosfj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pziwgfwl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yomrvujv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3evnjxogg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bcbyrhlv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ukhrdjuz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ntyndbxx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zugmfsce.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ybagpbzx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrbxijhh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rverfxge.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fdcyvkno.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lvzjkvjx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3orgubbau.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bmalzsgb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lbnorslu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wdrsugjh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ctaaiahe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dtcpxnpj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jqgzqzkn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3frxnaprv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnjxiuo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3brmmcqfi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jcoywugj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qqgdfrif.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fuxswzad.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3tgiyqnma.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3izsavfbk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yycvqdoj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jtyaoebt.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dswxmwmn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3anuiqjoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hneaxree.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nwvzwfai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toveuyfd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3javjducw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rzahfukd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wobhojyx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xmnuwbwf.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rjorwexf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3sdfbvoaq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rwauvhls.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3otaklrok.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nqvlcadb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mxkozefu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gcnbrzem.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ptosftwn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wryujybl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jtptvubo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bvwsbhcr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rzovdprq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wthavnup.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvxdxqy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3lmpxgppr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pubtxuar.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ewcajnev.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nprhngcu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xxtzehdx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3firnhwih.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rgrckmlx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kmtvlnvk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rlamlmkp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fyledjos.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3pgbnwqww.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bubbhtnn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ghnqbtuf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kgljossj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tlqcllzu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhidjwo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3zqlodulr.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kbuqtugz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zuacqhju.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmshrefl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ouqltffb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xuefwxbm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pymwbjcm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3uwndodxm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3titumubj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lptbulrb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nkhccsvk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oiogwbgp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fdeigqxa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vdnynaor.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3rmmaechw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvzfqub.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3plyzqpbr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqnqbqc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qhewbjwu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3flfxjnbh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3llgqvuon.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fkyweocy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nilhkmuj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3utrzkwiy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rawbkdks.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wqkhloym.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3pnbwymkx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3obevgbqb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vsfeydaj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wjsiswxt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zqevxxix.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3omgtqrql.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pmicznzi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3eviawyxt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3uovbfmls.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zfgjkyfk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xacaqgzq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tqzlqnvn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mlkfvhvs.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mgbiuglx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mppntlun.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mlxhpoyy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ubacyqsp.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3gkzfkivd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wjngorip.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jyweqftc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mpwjbver.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3moiueeem.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3gumltzuh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3cpitguup.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3huzrjpac.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ohbimyuu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pnwsdrbu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztbfopsj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqdmajwm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuokjktx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfaaqkib.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jkimkanp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3oqymvbgs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3rkiqkbeq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3toxzqmoj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3suhpppzq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3uwgivdur.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bgvdgmtg.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3tbjtljmr.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtvstugu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dfqhumoy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3mfoexckj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dhhwxsbd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hwgqhsqp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mqnwdudt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3tpmmjeig.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qwnwmnhb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3shhipgqo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lcrxhyzq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nqchfapv.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dlnfqsip.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmjrbtn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vfdrashh.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3sotinixw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cgmhlcnx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3hmfnxpmz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fuyehdyh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3efogliki.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3duvekhcn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ykllmwqt.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qrsbvjtq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3witgachj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3joxtsams.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3djehhmyl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lrhwajph.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zblhmshp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jfjqjfkm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cbocbecf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3fqqzjygw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wdgygdol.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3gdttzshe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cnarjdoh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rvgbniix.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3poansubw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3xbmyfvyl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvhskc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3iajtalov.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3wllvwcik.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3llfreixs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qsyvfqdr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3urlqndxt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lqszoeck.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3udemivpr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cqkkaoaa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mgyxmgpd.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hrdokgap.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tqnnrgrd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3sqygiuyc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3lodtabvn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fnazujpg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hcpdswnr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3lwmygcqx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3lrlyifdr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3pbloputm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3msxjsvrr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3izololln.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vhstzwap.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xscjrpjy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3djfpayoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vrxsbxiy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zjflzgow.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3alwifqsr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gezczyhw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fadbqeaq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jccbyhsn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lbjaodhj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3zdfvbbgs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fgwpooph.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gsympxve.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3liljgwlx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gwuvnxea.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sunveini.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jssgsqyn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iplgjfsb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ihatgujk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3amiybror.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3deyprqls.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jiqvyylm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ulhveklo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3uzwyzdte.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ibemzaji.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3japluwcl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hwqexcgo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewukdpqh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kesltdjf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3gllzsauv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wktzkumj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3khtciwcm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hbaxdlxk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3vyrjwmza.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bjlkhfnb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3poiysrnk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rbnfspzi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iwqwdfgz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3iylclpmq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qfhhbebm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rxhlklhb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ondlrybh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3usnzlbij.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3snydibvx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wlojjhsv.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mlijdrrw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3uapuizux.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3tafsjpbm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3qmeybwro.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jsnfwbhq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jrkglctx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ugjncqhk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wgkhupdf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yoybipsz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pgejdtyk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ijgcumjn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fbyuupma.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dfftihoq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3benkwani.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lvkqcigk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yodhudjd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3olyidueb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3edikikom.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3eoynagej.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tlizueun.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jxxsbqjy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3yrbpxtek.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bzsjtqel.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qptsznqc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3duiybhxe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qdsokycd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ksmviiwc.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3opkinfif.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mnxntwff.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3yolctxpi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3mnzcsgyi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zughptpf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kfzhpgeu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3moxyxlpv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qykxqjaj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tvpwxfaq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3nsbciujq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3chpnptos.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pstinxde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzujqxfy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ohgixaat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csfvzpub.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cxnbccoa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tdxhekkm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ldsokjpr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mqnlhnjp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ifikoqnc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aggnurgq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gwyhtxdn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ofvcbguk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3psretenm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xutlnyuk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wbsclpip.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gwgdevsj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3uwidccld.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eqrhulzp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3krxtizae.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ygpnkyyu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3avaepwqi.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3oeyjyvgn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fmjqbsvn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ttuqspfc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tjukcvxo.html


<!-- 参考信息 -->