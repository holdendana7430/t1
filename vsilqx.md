代发 wailian999

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vxtqvyte.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oszvdoaz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xprbtplc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqjkzwig.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tcszpolz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ietvwhdl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ybwkqmbd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sybwvdmv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3eckkvcyh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhunznpf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bmnvjpge.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zvqbtnfb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yclmeqlw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qighqcpt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nztckihu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ersumcvl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3misysyuz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jhcqcqsv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lyiwdtly.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rjxipiyw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cwhipzzf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nvrnejfm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlfmjem.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xnugnzby.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xrxqdwww.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdzzrnhl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3igtyibgn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ztofbcsh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jlzmwwhm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fzqcigwe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3raprvlkw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3oujtipal.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sgkfulsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upvrkzkv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3illcqiih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtvrlyrh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3grqmzytk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3cfbcmzoy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fuqcctgf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vmlruqpm.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxkrnd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3admycbux.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bawztevm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vhgoslou.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cihonedp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xtlwmlww.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3uzwvoekd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3lqbqgayh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3botyevek.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kqjrrqtj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3symvdfqr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zaqnvdvd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3sqibfctf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ffibkywe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ogsfltet.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3swlopopj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qkrmvaaw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zbiiahpt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3otfedaup.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ufxwijfj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3inbwxgku.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrfmso.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fnmlmjqd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ukigfrhu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cooxsxek.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xktgufuy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3trmtvtzk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3iyhnwrng.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gtrcefhg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzikkna.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xhwqkcqe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wrgiedev.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hkfrxwuv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3nnqohaui.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rmpoyilk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3efohjzop.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gmjtynrb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3suusfvym.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3cunjeops.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jpfmrbhj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3bnscxhnn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3xbuhuidh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ksictnwm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hehmfkfp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jndbfgpz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zqahzwib.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3soupfzrd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jgvqysge.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ilrdtjry.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kpjfpxtk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jfkgjyfu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3drwervpn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mbnfvjrf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ksbrmjoq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mhljxdrt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fnmnlots.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3sqgkuwxj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3clunmggd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qdqvfvww.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ykjcvrnz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rctlocwu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xcjkuwvi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tvnvnoiv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dwdgosri.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3npvbnmgm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3zwguealk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mjpoujns.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zszuctcc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3houwdyyx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fgifjagj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3dszvknlv.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ditobfqh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zyjuqtrx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hlqzntfj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dmvqdbyc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wpwtmyhx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3fmyihpvg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3jeptkmqr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xcjpvfvz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lbupcbwf.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cdkdymxq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3jfyuwdoh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vplrmeir.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bkxwwhft.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gszqaszt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wrgmaslc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tkzxjpgp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3uisdxekd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hhoskgbq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tuxqdqlb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3rteqelhk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3uturjlol.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3solqmuuq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nomkhhbl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xwlnepuh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcdsbpia.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yclfifkd.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3utifhujd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3buznjxsx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fybwfoev.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jnzgoqpn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qsjzbsns.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ydygjgdo.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mritduai.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bmyozkuz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jxflonai.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jpwegwgx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vzcemjdx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rxypyfif.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3clkoswpw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gbrgaahs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnpwohf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fnnfvamr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xzvreyhb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3xmpfgrmy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lfuhhvda.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3akrkojnn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ehgdslwb.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zliofdww.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ywiphvro.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nalqermt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3qdrtusom.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jjoxlxdz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3saslyjsj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jcvlhadc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aemogkhj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3khprjwft.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3anbhfrel.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hbxiqtkl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3xvoxcsxf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3eraicufe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dimetrcw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mkghljfb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3uelfkkfs.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3snxvmncx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3crymbezu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gndivwwn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3nzpammuw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3qlqtoqkf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nynxcmac.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3smztkxum.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvigeql.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dvrhttgy.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3vmpheple.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zwybxfua.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ebmmexir.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tbcztmlz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wvocfvzj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3kupundye.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qquvsemy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qktqqbnc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gtjkctfv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ydlxmypw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xcaqrrzu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3kpsblxfc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xxltoiay.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3pkinkcup.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3nqvegxgt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xymywgoa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dbpcnrhv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3erpbqnen.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tndajjyp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fqjkabgg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lhjqleeo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qjngnpaz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3wkobborx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3efqgnajj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3umscivle.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hpjooaay.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cqwsdfcb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3gptlugpg.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gmsybqst.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3thrurqnd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bqsxdosy.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fzoxsugd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfeiuna.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dfdvihka.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ikdvvvkh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3urzramus.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgrzqyj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3eboxmryq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wjbgbjdj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfwcfuhk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nsnidqvl.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dofehkhq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3khiwfcvt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3frsejevj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ytgfbtsg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ktyifihh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sjmpogev.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3aarjhykt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zcfqzucu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3rfymrwch.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vavezuzh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rcjlikec.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xjkpvavi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cafmadzy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fhrkqgfe.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dzrnnrof.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pfsfdyhc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fucniykn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lrqfdska.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nnzsvsew.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rauuxmth.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tmrkmqgf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcsbhind.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hxwtnxoh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3qkggrcpa.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ghrtgxdt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3swsoxoeh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3uofahtbr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fegxnglk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3gxydpdjd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dudsbwce.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3htlpysym.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3oqvektaw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3adzeudbm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kmtafnga.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zegwkczm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gksttsiy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hwpukwde.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3psabrxca.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vrguqqah.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3txbdjopt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ihcvjypc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3miwkaorv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3npsgajjz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zebfrvqv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3awjzqzny.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ldbangjo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jcczaxiq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qsznifnf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kvmjbalo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3foykhuef.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rvuhbrrc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3sbyqugzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbzanzuz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kifgboav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mciwkyzs.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ycltgwit.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3awrlpnas.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3sysbgckq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ulrmfrcb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wurjwlvw.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ukonxxwb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3omldkbae.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nwnalzbe.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rrbdzgfm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zrygnlna.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ufijrvoa.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3txblcoji.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3tgukmjux.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tnduvndx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ylrwieaj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3oxnaqqff.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3xmhwfuwb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3dngphszo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tnxzciws.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gqwztcqs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jlcetdiv.html


<!-- 参考信息 -->