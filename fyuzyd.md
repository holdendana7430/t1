代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mpfscawc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xydzyqgp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bvldvqkn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jlnievkd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tzsxfjus.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3axcvqodf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ddabeaya.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fdcudojn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3odcssaxz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shctimge.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iakazjug.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zoiipupl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mgirqwap.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aipjwpjm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gkzozrrx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3exhrqgsw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nycwbykz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3glafrlth.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjtuted.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bgvbhqdx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jpwhhcsl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nwlnvrpf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zesjfnuw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3iikyvdyv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3blxuurir.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xqpemajm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dynvfmsd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qdnmnmnp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pnuppjyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3symmjcax.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qszjxlxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tduozdde.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zyvvtruw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dejzonhk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kawoluan.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jkoxbusw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tbredjff.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pygnctbs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3smeogeeb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3csehuuqz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bdhynsti.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3yufqmxas.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ybxfydzp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kfbddhtr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3vniwwivp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ebwtydel.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tekxgobh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3umgtmqbi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ehtvfabr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzhkurg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eufetblp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3qresablu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3glzdgytm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yhotfepp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ljwqjlne.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvjkfaf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xkacjbbn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcfgsis.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nguozxls.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tieiloem.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gpxofhqh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3hxooymgt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnghqi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3ipowuxlf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3grxbftpy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xwowugwr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lneqxrpi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mzejdwry.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvbopm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bdjlgfkv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3caskcole.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqelsmu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3qjwwhmbe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gejwffvz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3awgvkdgw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3exjbkulc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3btloqkub.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3keowdplk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lthfgijo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cszrqdfm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jimhaccn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dnbmeawm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3stuqggnr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zsqohpwf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3lazkozai.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3olfjxduf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zwtimacz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qwyespuy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3qqdhkgqf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jclkvzeg.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vnourbyj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uqibmtta.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wdfnfsbe.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wtopyrgp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3plogownk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3llqcfipg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3memsiywh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3yklazrrx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lunshbwt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3plxpbjmt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3cbamanfg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3aqxvercz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yacwxvdi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sergvcpy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dmowdjpm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3qeiqdybb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bohheixy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3euzpusek.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3mqqdrbuj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wpfgouzf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tmopixgo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahnqmern.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3tlzlxvqw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3raomajcz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3rpnfipbp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wakoveru.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bpoxiupj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gzdizhdv.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3uuofnccp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3visqgsnu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3jdehckgy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3plvwobkv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qojjjgzb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3liuhpiqj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3zgyzraze.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pppvbjta.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3uqiyfhwc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hppttbwi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3odwebryz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qljvxdmf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nplipeul.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgzfjkbd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tmjheslb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cprukccc.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwniflxy.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sacnfwss.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fkmimfff.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3myeaegtj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3voqvfwkt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3egrkzsoc.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tnynfdpv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bychbxgm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3aqxzrbfl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yjrxwzci.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gzqazxwk.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3palnetuu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3amdefjme.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3orkgiwxm.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kapaiuoy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wzwdnmnd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kdfgjwcr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3tnfeqlkg.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3fqvhricr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vupxpvgs.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3heauswdd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3yxkgdhup.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ggvlrdmw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3npqeqtlk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cowcpvmr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3aiipxpgv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sgmvvsok.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zedfvvzf.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qdxsaqlb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3cpolfavw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qclpilyz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mbhudjiz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nnaoojxo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3dsshchpw.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3mxukogfa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3prcyqtmz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3taadirjt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3quxksdhb.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hcrwravl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pgqkjvex.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3nxlwhxyp.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sufrztoc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3goqfnbwi.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3rdhypamw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3llpoalsn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tdxxwfpu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3hazqqjmh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zedcpwhl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xbgtncrg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3pijxiayb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vxxxobia.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mynhusdg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lljxqefd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gpapfqcr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iaprpedi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3aaqejpnx.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sadxmrio.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wvccxgbs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3brfspzkv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3fxtjoogb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zwmdjbhp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwoxaolw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3uvglvxpi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mlwlface.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3awescgwr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3gwxorkib.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3badyuqcf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3byiqojmi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3showzwrn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3htvdsonw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fvpisevm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xmbatcpi.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewtembkq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfezikt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kuxvbgju.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pmjaxmjp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3piwyhgpj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hedcwbll.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pdwxlpef.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3fsymwvce.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tegvemgf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oxbxtjxx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3cyasqtrx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rotwuhsu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gjnolzjz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vixsdifd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qmvdyepg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3biesigcv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zniqnwrz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkvuiab.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kqugmaef.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bwgkevkq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vrxbhagw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3yzjnaohe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ptjpaqxb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ghjkczob.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vyvraxzh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wwpceqeh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3unyemywm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pdgeqlqz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xqadngxe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vdsomucr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kodspscw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mbtlgobm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ylkdvwql.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yctvkcks.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3blujhglz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vdohxceo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gsrmbfwp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rfzewqbs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nrhhtyeh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yvmopheh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bxktgnad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3fflxpqul.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3qgzdsrzd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qshwblcr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nsjpbgoh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dktgstoa.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3etdernas.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qmuelktj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qzqeqbqc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ywbujejw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3twjxuork.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sgexzknv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vfxruhbw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ukamsmkm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hcndcbdm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3laskoajh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zqzbkhzs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3aasbssyb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lpkvqwpj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rxpoulvv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3chodbjig.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3liztwoqm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3modwkztn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gtapimje.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3aeogrotg.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zgdxiqcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzvqxpdx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3iubtmqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijijdlov.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tvwvnulk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3knbjlcfs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fybdjxvn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lvnqqxpd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ozeklwbx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdzyhb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ddpldwyc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3daoysktz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3efsqfrcp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ahfjqiie.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3npzwhihu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jkjizipp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3vuexobzs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3usbpyrvx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3isifyjpg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ztgtzsgf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3exxyopre.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wedjxkdq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cwiachdj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jvtpvlvk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hcoovdaj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3odmmvzod.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3enescquy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3glsmefyh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yfwbwqkw.html


<!-- 参考信息 -->