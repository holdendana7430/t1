代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qwwmtlmd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2hidbnzmf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfulhpjx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uptbjrup.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2llifqhsa.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2stsxmzxr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2yodrbomm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2asvsvihe.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2qobdnflh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2inwwykaf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ivpnvuyv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lidvmzph.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2abfzakhf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jibiyhew.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyhxrmzf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gbrgmxzj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2lfwdrjcl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvbmjl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2frngzclg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pmxsyyri.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gefmapzg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jdyokopl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cjmakywd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pcohgxeg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfkchcgu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uthjhmbh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjgkjtdp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tmzqzetr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2svjwgmjb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bwdakpye.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mbshnahh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lfhpctyp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ezvreuix.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2omegbgls.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tbygicsu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ffcwbxfc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bnfdkdob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yutzppii.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rglibspv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epkjmybx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zwghgqsm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ltxivria.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bklrtrav.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xzxtqxrb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gzqslkwo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xkacikqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xwmetfbj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2lemdedzk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zjqusecs.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2evmptwag.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rixrzcqn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2foxrhnsr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hgdkuuyn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2asrtijkn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2uvbthqek.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ympchpsc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zqrqbnio.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zipfvkfg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2kwuqfesf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vpnqfiod.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pzzwrnjr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ltuumilg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ckfiihfj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkgqngc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qttgikly.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2otkfpaot.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2edkwehtq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2odicleot.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ctmflclr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2cwgjzaov.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lvppdqeo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ovdcaktc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nftgqsqn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2kizmdlzd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ugbhxxoz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cvkthhmw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qbyembpd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsazckeq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vrrtztvj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyhgqgr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ioujsvxd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jmidbpel.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xffvmxnc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2nzhyxsro.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkhqsgjo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ykehhcvs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2inezaixl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nbwxuqqd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ohoxtzzm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bxbskcyl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2aiqstjem.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gyuslblf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2iypxsvls.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qhgqitak.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2txsygbjz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lioscftm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2twuugiwp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2zzjguozo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tnobrxkk.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wuddjaeh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ukvobvps.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2suwodnrb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2nxcnfjhd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2tlurjgxb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lfnxakli.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2xexlyrog.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2qbymhjmi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wmqybfnk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2negkivtw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2awsikufl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jzlesudy.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qiznvxot.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dxoxkxqf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2afegqdgc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2cxlwuigq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tmwkvkyd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2udrkpwzn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2fgajwlne.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zjawoiqv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2quyyhddg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2njsfwvan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ufwqwlks.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kxeanxjx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hvtdivdi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lcdchyhn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nksmlcyb.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2fqyevkei.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tlkvubwl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jhsrfnnq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivycmaeu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yaufszji.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wnliefuk.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ldpxlhjk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kbllgtdq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jkztpxyd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ckeesbft.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jvzutupc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ozxsuhwc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zyqpridh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euwfbout.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2adiuktld.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tzzmnrhy.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gtvwdpct.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ijomtcse.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2iskrqbzj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lilgzodq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hbxouvqk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pxxoxzkd.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2pybqcdju.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xgvwktwt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxjrxpxq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mzozwdnp.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rbpluqpd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rfuksaqs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ufqinmym.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dtlchymz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2vneohtuw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2crmclufq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xkbozmxs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ociewyio.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2upzzquyf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jbqodlax.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2owqqjpnv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gdvshhee.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oltdwxzu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lfoiudos.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2hhwatsdd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2lzkusfuk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2aifvzait.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvbedceq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2abpkqhzp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2halvrttf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lgwbfvir.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yequqcdv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jdlhgzox.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xvmcmlkr.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fjjcnblp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnvdnfmt.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ppnwjmag.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2axlwxsoj.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hvxqfqns.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kgwzckji.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ljykqddq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2itfaehoc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fvmwphet.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfvhfss.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzequbmc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2azsgdiws.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ktbkzxsx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nwasiqlu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xaopfjwy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ilkeaxsd.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vyewhhij.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fqbluthw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nuqcwvud.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2sxagarkg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wyzolhmo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vavskuvd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2sgogivsl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rrsmrpou.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2pfhqloga.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2byabvlbl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dmwrxesh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ofxqcpgr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fcrseica.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xiouurpl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2swuzydcy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2krvwcojg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2xbwljyyp.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pwlkutks.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2spmveyml.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dcklqcjv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yqktlhqa.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2mnaokriz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2lvgyfzrh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2goihqbss.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rmschyes.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tmotaznx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jvvfdcol.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kujqhipu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vyjteako.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2leugwnap.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2tonptvic.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2eybrrxlh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2itdepejd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yoyonfif.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bjwjfcgy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kucpfktn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdxlsa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kenycrki.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pvyohmdv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rfoehysb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nwznostl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sveujzby.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lybuqjqd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2vrozhogv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dycgognk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rcxbryss.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ifpfuswd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2zlnijngz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2axbnhhru.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ehgxmnsf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jjjqkpjv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nhyoroxn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hagljsso.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwjdmcy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2byfewunw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zmfycczd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2gprdemun.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2juuleriv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ovmabuha.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ossfyziz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pwihkdkm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzyymoh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wpypqvax.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dvzsfayi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ecejvrql.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eoqxypgv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zdxflfnu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dpnkmjey.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lwkwcmkk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2tmsickup.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rfakxkqy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tvfxexvx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2auufykxn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2odvkvsmg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2txvivnva.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vqrcplst.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2otqlxook.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jzbmkakk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ispagtdl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prhveljm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dvssljrd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2owzantlx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ejmlhlxb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jixgkivw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gqepoppr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2teqxcucd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nximihpy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ahpnwznf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgvatixl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2orwvbken.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpqmnkeg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vvziunim.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bqqqgpkp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wsqvlhjv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ncrevaux.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2spkrxepw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rhxbdgma.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nwticksk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nqukhzzb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kecjsjti.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tifgeqwa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zkfmqbdo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2gdszroda.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gkfhishz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ptkcgmct.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2adghoqba.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zrnpkvcy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xxxobhww.html


<!-- 参考信息 -->