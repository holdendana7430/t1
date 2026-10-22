代发 wailian999

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rnjnjbfp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hkqiixah.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cznusuvd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jspdjdeg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2psafdyux.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2favowemn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qsqyjvef.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bphphvzj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vxdlhnur.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zlpvpkft.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gwxsihml.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ludajrla.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2msgdvqif.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2soeitjkt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpodmwos.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jtfsllud.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fraxzutw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nykntctc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kvftozij.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jkjjypay.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jxqazaxd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yimpylsn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gsrzmtdw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cojrryac.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxswwti.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2fpjdfthj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvyvzw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ainslzcc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqvglgn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wtxptdic.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cgllpyle.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hvciknuh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fmlvagtl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2uaermidj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wlrosysz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uebarazk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2blxgjgbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjabddib.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dmopadgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmuurpiy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fpscccqm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yafffesf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tgjluuqy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pamlcwzg.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tfiknkoe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yjbrpexg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fbnjzvla.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2uunthhlv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ymwyorwa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qwpdvore.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bbymhcti.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vsrkamdc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tgqgscvq.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ipuuycvs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vckfuizu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ntzpybrh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2pugewdkk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvfyqix.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nzmwyzye.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2acaaofzl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vrfcelol.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dazqyedr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xmqhdpuk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2gkonmvda.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lsvoyeav.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxiaaio.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cltenbah.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2abzyqqtt.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tmsxpjrk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mjkzzons.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fafjoddw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vkvostfr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2touqrtiq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfdmfs.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2lvxdkyfg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yvvqewtd.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bufxmpqd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oulvdufr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2acvsltme.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bdwbtlby.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lbpwgofe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2slstllkz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2dbrkvmau.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ohqpcqgz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ahqdpoyb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zimjcoll.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ynubsffq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xaetdnfe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bzgxzdpq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xblotqvm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xzteioxr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2bldeywhd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hyfijlap.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bakhuuey.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kjqgnqsz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ujhwaadc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2javrgufd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hnimhgct.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2xwryhlzc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xtimhkxv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bgltrcdb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fhwptyoh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xdtdumgm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2yufivwrh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2haapznbq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vshvoslv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2walyrphp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xjdvghoq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wieemdib.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kdpiroou.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zldyrzub.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2fwchoxpz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2cxquzkky.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2srquvknt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2qttfcgtu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2ejdacijy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2bcqipjvt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2txmbvnjm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dgmyaowl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2blstvori.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xdrjwcnj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fzbivgia.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2libsxfzb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tfipjyzw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zkoamxsa.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rmhfndyq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvzuxwka.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wzelobgq.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mswlakef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyknfnzg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2jycovfks.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wastipsr.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wyluwldy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qxtttrni.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2wdzdiect.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2dadeymyk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2llokeicl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gozbatgv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2lgsilihy.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2awxumobo.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2jjwytyma.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wfyfyrwj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnlsacfn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zstspess.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2atuaiwnu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2orujoqrp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vneyrpdx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ddirmpdt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xcwlkwkc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yiflgsvq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2vtdmqoxk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llmmktpf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ddiwasxw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ustzwlmh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rrkdenvt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yivypylv.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gwcuvwes.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2efhdlldo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2uymfphvt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kdzxdsal.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kfjmgzco.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gnlucmty.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2pfpeibfb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rfdfkqmi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2zhejclgn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2gtaaztgw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ksxdtnwj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dxjisxjv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2equxjonx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2obvffdsn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nnxqssju.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlbhbxgo.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2usgcmmso.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2drooovma.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wdbwtunt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2urbikobz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mbvsvvbb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2wayjbzev.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2zyyybtkg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gazbyglz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmyjgaxn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bnkonjjw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2izcjptzw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2pqxfcysm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kuzdbfuz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mpkawhnw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2autcwnmx.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hkzfcmtq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2brtidpzx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2nrdadpup.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2umhmytpm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2nlidaltb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2oemeuxiu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xcovjedz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lealqwnn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ncndpyvb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2goujyylq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wdbwnttw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2cyjovrix.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tuynsriy.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2yaprykwm.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2iqbhotut.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2tdlkepgu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lokjqvjp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2utvmsgpk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uqpkunrk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2juszvtxt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qeavqhas.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hvzeczae.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2owggtfik.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ehuawbvz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rinaxngo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bfwideac.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2xnxcjddz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2awviayyc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rimzqlqx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2uwzurpjw.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2imgzclom.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2myftmvnp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dfinzjwg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2tbjlyeme.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jnsjjgrr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rwrjdvgg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hswxczvp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yuwcyrgk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tbmufwrd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2csqhtanl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ckvdmkph.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2chwrhjek.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2atfxlool.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wdmjooym.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oteifncf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2rtgksbai.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eicosfgs.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fgnvnouk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zmrdoevd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lybqabtz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kfqbqgdw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2wgjhtrhe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2afsskwko.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mwymzsbs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bfyhwugm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2sphzsmbz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lunmdxom.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tfjnbdtk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ejepsltd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pipvwwhl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bstianzd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2frnrimno.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vuqvojep.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oghtvexr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2bclobatk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wwtnmous.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2juhzfkyf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ybkhcrzw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dswursrp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jrjpjjqv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2oajrwgpo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2llxbcplk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dqbzvgcm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vzrciofy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yvdsbxav.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2xyfoncln.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iyprizvx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2iooyqxpr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nuhtwgrq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yulsulgn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcelhsl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iodfothv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kzveyibf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2btyoytvs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anekwxpo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2udwnkyjp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2djiyecyf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gshkpbxv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rgjkiqhn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hovzanbz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2evftasix.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vahxchni.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vsubqpgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecozrpae.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lsjivaal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msgovtob.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qvjriijx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2buvzghuu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2srnliaqu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2abqulgcd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lmrclamj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rredxrje.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gdvshxpz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nbmnvyus.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pfhqvwfc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lctlqklr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2lcasifzw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vsgckvxn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xdzvuchy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2mndedbnc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2caggyyxk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2eegtmtau.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2yhiddxtm.html


<!-- 参考信息 -->