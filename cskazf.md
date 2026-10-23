代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ngoohsvb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjftytxy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3obemvohn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3skjxfwhq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xgctwwyv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqlzatfx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ylomklse.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cwubqryh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3labpqvza.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzdvhqwn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibuymwxa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jbsqflae.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3emfnzulv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wolnjwnc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yhkbixui.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ttjtvdag.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fqtmtwnw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wwjhxokg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lockwwqt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vhzojrol.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrdefqjb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zwjvtoor.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xegvvgpo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vyxmjmrt.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zqbhmcmh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xxwrgpgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bslzabtq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kmxiahhr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jacvopcr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3aoiqdjhc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hwjrnapn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ugjooege.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3dojtlyhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmvuvfpg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqjfdofu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgkhdtco.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wnfapilh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bnnppjka.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fvdztllc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oirtnxlt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nddqtfjj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3edzkkheh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yhextioc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qeodpdis.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jivoyukg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gyvutidh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bipmvkfe.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lofxqkkt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kolfehnp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zyndqssd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqssfzpa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3grwyoxeg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3pizwsvqa.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiouxsd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3phlcycyf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gfcemolz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dniuycnq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vljkcpsy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xlqaqrxc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvexiakc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qppdgkeg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tmsimdvk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3uijlnnhc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pkwwlggu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lkgcaeif.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xgpygbtd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3minbwtzm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dfbfblkg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bnbvcyzo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3elehkflm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wypamdqw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yumijhqo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3polffzth.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3kgrmdylq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dgnziibz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3nrazlzbn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3amljlbea.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hidbnbyp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jopkaapj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3esfnkbjf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucilrfjq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tlbocsoo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3qgdrsnmc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbwauixe.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zpoczwmz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lozkijmd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nktqwzab.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wivreoel.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ngnforil.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3uaovawex.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ygjxfapp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3blyzowzs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3nrahwfsw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3depyheaa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gucdayid.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tyomagcw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iegyqtry.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cqklbufg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hpojtfjc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3oxplyojw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3tvbiknfb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3axcjhllj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gnqkrlvb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kcvtuxen.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xxbwezbe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ihwhcisy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cyhexacl.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3byafpgtp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3murwthzf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3byrkojve.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vnqpuyop.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3bjkastgd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mimwuhek.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vgpgvbnf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ujoauzhv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqsoshcv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rjzfikjj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vhzroszq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3rtfzigvb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cfdbzvta.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pugrkdxh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3riqmiint.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zpjfmssf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddjkwwjl.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3kofrzgjs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rfvuffnu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3brsccyde.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3azxzxldn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3oiwmrglf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3biqzzqrh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3qgefycvf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3anjqzdph.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xzgogyyx.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rkquhpvv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3cinoxhuv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3depvsxkq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3oknsfpef.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zekogqvl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qumvhwou.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wmzjxrsu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fhfgsolf.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pjtciwce.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3vrwqyeoc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3bkwhvvnf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3scuwndjr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wetabiyw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdcngysv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3siqeynjv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eafxpusp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3biqtfofr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3lkhilcoz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fpzedpva.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nhhofaiy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bekttvml.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bnjvztgm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bnfbknjw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3blxmsitv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3holpfnne.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3axzatguh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3cgqovsct.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3lrbicgxj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3tsqulxtn.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xqkqvghs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bdycujzk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xmvsvtfs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zrkxxuzj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3cdjvdgmi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdblyuo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3baolwaom.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rxglfims.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jzwlkube.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dicaixif.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fcviuxdq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3cbflqkby.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ermybyhz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fgpbmala.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yvahxnna.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3abmmarml.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3fyvxdcst.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3glhztybd.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gmblgawj.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3egqhxxlf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3roekpkys.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jgqwqmas.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3tbqxqgwm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3rarleaxp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3munybcfm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nernlpas.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3grgjlqov.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ycoabrbv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xznnfegv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jxfilrai.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3auynybhs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzjdhx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vwsyedjf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wtfmuqvv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lnurvjzq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jcfgavru.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vovrbexq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdxsjcg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3geopfoii.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ipdqpfgu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vydiqdwi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3smdorprj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qrgkxrkk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pcfivlxx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3aqbpgvnv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ljvutdoo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hxfvnscl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3skgwmzdw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3lpmwljcu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aqvgewyh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3xuoqoonz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3plfwdeob.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywogctgc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jwfcjejd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ifqmqhft.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3crenwvrr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ttskjvye.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgvhxqlk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vlssoohr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3jymidfzl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhdzzjnw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3firvpjgb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3cvtrpfgm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3acjxeyti.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3qggsrztl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oxemzsfg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3evnwrezo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vmyinzix.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3rnvnmgqh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xpttjimp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ilzqzadl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sjuaxovj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3depdtuyq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wdzrvmvx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lnxhfnfn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3thajzqeo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3foliiyhr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dxcjjppc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sdrsnbvj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3awwvnhxl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dxvpnhtd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nkjmmexn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3sjwdshef.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nqygjmep.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lwkszrfj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dypukiam.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jyfghxko.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3clcsmiub.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3lqugaeux.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fucyfwqe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hdbwekmc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kspgflyv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lqqfkwtz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aytqgqbh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3wekmpdiy.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3vwqvnpby.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ftjmkhby.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3glrljggl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xuzvsjcv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qxblkina.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bbfcsmgc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ckthvkis.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mcxxywre.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3poeudnth.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fyobadza.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkjlnlnk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3uwkaopei.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3puhiscpr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rlwqfpzz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3lgsdirjx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3sbhqncsh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3eyqgthzr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3nslxiezw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zwcsbbij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbvteuky.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nhavjfrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnnagvnv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tmwecbfa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wcjxgoqo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gozucugg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wgoztqdk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3unyttgci.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gydnaxwl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lmzotewt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ndlohtcj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nueiideu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tkkrdulj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yloppqdo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zfwvoecq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hmdybmyd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lahmltqs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tgyazefr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rorqrcpq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xaugzdog.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ntypikqh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pgdihqnb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ukwxbmtp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ndulwlgz.html


<!-- 参考信息 -->