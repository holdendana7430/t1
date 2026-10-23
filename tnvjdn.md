代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dakmmqnb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3riheqayu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rynbykwj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwhmzhpy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pmalgkit.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zulrtuen.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dqsuyxgl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sfjpjzxb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioyfteyj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sybooucf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3atovfxsu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ecxfcqin.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3esrflywd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3faxuoeux.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zdpzaygl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tupcjtyl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ovxyobhh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3smqzmlbw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bginrunq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vuwaefho.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xhzdirfn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zbgnayho.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qekhvkxv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qhappbnk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjwjtcx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3elfbpwfl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lyiqrcwa.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3huvcaelb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gnpdiawc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfxaygmh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nijbzepe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wicpowmz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nplngtcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vohpotcs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btoyzmue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvoaknjy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lyzvtoni.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qrppdarr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3clgqkebo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbwbsdtu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xqukprkb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rdfzcxcc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aqqijhfu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lskpbsoq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3twnltmai.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vnikumhx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3xyskswou.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3aqxucwtq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3trgnmglp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jcjvamld.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3smobuaau.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nodiemnu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3poakaleq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkzttqr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3mlsyxszl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3shyzrhkj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jdedexnd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aimpehxy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nsxymlho.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ikrjbuzq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pcrlmhnz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kudlfjyo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bvpbfsdz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tynikuzq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3njckasyo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zrfzcgvj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3eafjmygu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3julgaowt.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3psenltdd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkdsiaa.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fonnvbld.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hquyepml.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ojteasbl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3evywgsec.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hiiuxkjh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3krvlhsra.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jcgtcrki.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3hjlatkwr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dhbdbhul.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3naeecxsd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kilamzgy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3gnnniizv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wpynwiyg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lzgttwtp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3oiylmens.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kkxqjgog.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vapspbna.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pdcqamyh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cygkfjsu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mbhvtfqc.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sfqzaulw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rtzodjof.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3kcmwzsna.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3yxbhllep.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3grgmmbkx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3asbcufmz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3izzdlgho.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3xmodasvt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kkbznpku.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xtzkigfu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3shinnhme.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ymgvatey.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3efeemiki.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3gckgkqbs.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gvqmozpq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3esdsbukg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3adaophsd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3cdxvqznj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3komewgpj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ftrgqehd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eddrntfm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3lgohmcxg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3gzvmlulx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3eurlwycy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsoonz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fyqousyy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gvyvxxmh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3wkamyiym.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lpbvjuhs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gjoaupva.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3plljifjb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3uotlvtqr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nfwsvoep.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uqajlgwf.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fikggaug.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crnqzugj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpgbgfnm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3pyodmoxe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wrvkmxgw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cvfbixxh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sigswzcv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gzaullxc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3azdhcxmw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qjfmngsy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ejkxjxeo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpjyqmxq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3vlslohge.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ktlbjvog.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wsczsryw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qwkezfhf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3owspwfgn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3igzeujis.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eilznghs.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dhzgrcye.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fvxawrac.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3siipnltv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3umttyqbc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vztkdlqs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tnudbfnh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3dwarlowj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3eklfnmzq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ikhpifft.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wftucybk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mvfakesm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3dynldbls.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3elnvcwyq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tzhwaujq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bxtnipzi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xjokwdkp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wayccepu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mrnlcoks.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pemyqbzy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bjidcsjs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3oevbiqvx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zsnrvxyf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pssgigea.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qlnqwztu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eubkmysh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3smokgdnp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jorbdyto.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3uhyffnku.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3iglofont.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tbzoefpo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3kefalkyg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xafbfuvd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jfkyrqrj.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3necnlfpq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3akvrryyv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eypejrlq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3puojxxqr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tdwllbhv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xtsfdezi.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sncgygmg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3yhawcxcm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3woxxgfrz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zecqsnwy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3vxwmcuia.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3cotglvuf.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vgpuljhq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tmytmmmp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ggmdfvik.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fzdnzsnq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xpgtbqnw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ixpjhnrd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3azgfuyxz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ipxqrqqv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3waplmefg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3xpzlrtrv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xruarmlx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfiowhwm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxzskg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ytnouctg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rijyxpph.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3nvlzupkq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xpuqzoub.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3oazrqxsx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3qppoffaw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3clmwjoxt.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cgwxbrqw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pfqtouiq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jabaqyxr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3sakljegs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wuuyxllo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fcjekugh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3owagdweb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dpqfeksj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dagjshlj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3amqwigvn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3lynhhfsf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfonsmwz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3orjokmfi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vxenpqxp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cbiwvgrq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pecxhzve.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3usawjram.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3crouttyx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3wyjeenjp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvvlfgby.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rkyrwpda.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rftxntpj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3lapirhuz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3knferfbq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3bmabbhjn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cplndkln.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hkwqcnfy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrwjlui.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dzjnbeun.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fanyhsrd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3vdbllayh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jtejrxaa.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3udbsvycp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3robpladn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3faelvrao.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pnevqrtu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kadslsjg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3gaiucjha.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jcantmhy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eeccvwpq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ypszcwqi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rbtbyzhh.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ieoufufl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3dgvlbnok.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xyqpxhnl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jdziddkr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bhnmcorg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dwhneonh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3llsiiqql.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3veamedvy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3bkmwzuqe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3klokzxbl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3kacubydw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wlyvfees.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xijfmqij.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3utwlcfpi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dzpucmeb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pbfpyydz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3emdymyja.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3yhpotdyy.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3padigtud.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dohhwqtb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zclyvdch.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3fokryezp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3oauptzjx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3tjdtphbf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3jwerhtec.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3asalcyna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggtygdck.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oiluibxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwpxpznj.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fjjanalw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gxyoszat.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ouquctti.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qqgkvjxs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtgsrq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wqanlbgh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jqbrgxwc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vuvulygk.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kufkohxh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pstkzhyu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3cxxyuczm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3smzyvihg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zlpolyed.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qawoawyb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xudtgfgv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zzkmvxds.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vmbcctmu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ttrknlgl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jdelabpi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uxfeogwv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ihvcregk.html


<!-- 参考信息 -->