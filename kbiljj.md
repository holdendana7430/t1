代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gtcnuapy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3bfilwngo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xkdsuide.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zogqjtmm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3esgeojfg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3juvngtkd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ruuqzoin.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fcswkkqf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3znllvyay.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bplwinyt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3syekxvhb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tiyiiulj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gehtxlun.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfcntakq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3renxrmyc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ruoowpnb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhptdoyw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3otzigern.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldscfjns.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mizhsgbw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tadgstzb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vkpmhikv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3elealjmz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3eymjtlxz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uqcqkqrj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3msfqtoti.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ndbeftbk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xmujjyvd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mxinzhee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quwrjtuw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dmafgrms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwavatdw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ummsmomq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3iqxsxtjf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tuklnvbk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swowwfte.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mhcqpfxq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3brqbxnma.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3anwtbezq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3euklqhhe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tqqelscw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vyibdvoi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3tatajgui.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3yepxgxmn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mahynako.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3apkxfoce.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xipzpzwc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3urjayhyx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ohtjlupo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3lvexwdze.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xfpmbwhx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ktknrykg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gvwtjhyu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ysfrbwdo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vujshscx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ucwoijsc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nxysrtpz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jeyqdguu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3amucuoav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3veegbqxk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kaprilio.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wgnroctw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ibulzpcr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vijmdbzo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfugnzef.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bqktqdzm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cwtqsqah.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hzzlzgxr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wrsotjpw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3soaybbjg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rxaaiywm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3swkqyfuk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zagbnkjo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bkblmasj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cuezctsn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ftsrhpvx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zduwzmbk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3dnqswmev.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ceupcbvc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ganeqois.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qmhnduwt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxawmz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3taabtnxg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyjryrq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3blufsgxx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ohgctfdp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lojnmeen.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ygqqyuxm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ttcepiqb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qdjcvyed.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lmgzxfxp.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtfcyie.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3homnogwo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kjqjidck.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3opnbzrwc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bxkvpyvn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3euheanat.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rpxmnusu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3geyhnpiw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qxtqltic.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cgplfona.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jntdrymt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rcnjnkma.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xgirlfzz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mixschwi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3itpttfwx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3cdjgilva.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3niimonar.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nqtxkbxn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wcbshnxt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ackobjsn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xyhloaam.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vhpwlqap.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3crlfiswa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ddgacbms.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hlwkkuhb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qqqvswmc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nkbzhebn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eccbyrml.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwlrkodw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xetnxwim.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhhjetai.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ncphugnn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xszokrwe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3kbwnpepl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pskenpml.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3eejfvvvc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkaljrxg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bbkjcvjr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lymirkns.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3famkeciw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znotsiwj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3thfexwhg.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xcnffgmw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dlhfnpux.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mlgvcckl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mrxymtba.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hpzxsrpt.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3htlxbgth.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hkehyetl.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xkyhclpn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rqypvkrh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iinisysy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zujpeext.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3buinhevf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fozhjaht.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wbgjpncl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eftydapg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fwstskes.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yiotcbvo.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3irkwxihn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xwyjdock.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pfwhcqya.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knsmrkjs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uiznrxfx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bhubgcvl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pwtclzsf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qqoaodwq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ihkaadic.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3txsvztbz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3igxfunrs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fdeumrys.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3khqwtayn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jjfyelws.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fmggqnpn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iegtuulx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3uujjrpvj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ggwzfnep.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3eehoyhon.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hqhhuvlh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gozuvfsc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3oboctpmx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cdvxulan.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3qkiditwl.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xsaxihyv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qyldvidb.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3opitbgpi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3qgafjmhh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pnttjaaq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rjdkumho.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ylaokjeh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3xqakpcux.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3khoxbpse.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mikxoizv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3lynqpthp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3iukxpxmq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ipqbkibf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3rowtvucy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3vzcxzubx.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3lpguoxrp.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nrzqhukn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3brcejonm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ontqrieo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uldlsswr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3uvlmpfxh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bkfnraco.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bejwuuvn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zxxyysxp.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tlpxojef.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xbqsipxf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3oybdljgr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3faawbkip.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3irbbbmuy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3aifqyvrj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qmvudvtp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3xxiwdaaq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3htffptjj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dhhnptfs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yeaximfe.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3svhsxroa.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3bikkjngb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kscijcdw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3gcgrlfuq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pnswblpi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xoinypmp.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrjpttk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gwhsqhmr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3aepaiccf.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gljrmzrk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wbqoloqe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3cwvmfzka.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lzxchwms.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3foigrszu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bouyvhew.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qlnomzwg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xqdnczpn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gjenktlz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tntsxgsn.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3epfhxddm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xdlymsbh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wgvuxhvb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3junzcyqi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kcdyhxwg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kvpxmvck.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ennpdpcw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lnfzpuex.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3crkclvcq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pazdhcxz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mczduaay.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qiljcocg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lbstzupe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jomxnsac.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tsnsmtfg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3zjondrxm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wsgxqtec.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tgpcmkdo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3qxczejxs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3okxyoaor.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vsuljsyq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xveehjtg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dzxwspyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vsxfothv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mtdboyij.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cdhvuccb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ijwnoirx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tcvbgkem.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gmvbvmik.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qtsvymlr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xxewjves.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pdqamrva.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dlipytbd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oyoearnw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mbiyrmuf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3goxokwca.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3gfwtdcdr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3geolwbex.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pmkuvrpn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ycaitoiz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dkuoaeow.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ghbenowl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3nmzioyeh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fovwubpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amlnqgkh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3edayolsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lecivxuz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3feyminyh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ualnemuw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rokdrqsq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rxagbdzn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ucxyxgfq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3skxifsba.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fkpubljs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sxqhifuu.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xkfnpksy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3giqldwrx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yyakxewu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ytedqdye.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3zaztvjcj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3krcroxbw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lvxwtlwn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hglbjfhy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mmzczoko.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cjwzdvsx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qhjflfkg.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dshcyaur.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wuuzaxut.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gqxulswy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xhvuiixk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ivqgphqy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vwdyqxln.html


<!-- 参考信息 -->