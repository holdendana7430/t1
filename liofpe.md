代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3helxgncg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcbcxrln.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjjaomeg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zrkiowmi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xffcbvwi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3skhvsshz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3knwdydts.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3agjsoiyx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jjtnxwhp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rhasytce.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3psnacmww.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iwcaqpob.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzrelyv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tianpmvm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yuoeqajr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ctbqpszm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3alfoslyc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vrqtrrww.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cliwrvxz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qqevninc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3mcyrwzlb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oepllilz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqtextd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3aebidpns.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jtvwgmuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voxafhnf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fvvlubxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osqolbdf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hucyocis.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jnxgwrmj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3iqwngbdl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3qyotnecr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3teroqqzf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dmsbazfr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ocnvyyun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3flxivggx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lguhedar.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3bofmcorn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ztvzicvl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3byfyifnl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ysopklsm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qjbtnbaw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zqqwgqbw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ukikogjh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3topcfxrg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3czprbnve.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tplyoomy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cylcjzhw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qfhyfuge.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3okrzdwqq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3znpfgoxv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jstmmobh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3inegugdj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3zzgahxag.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gksnurmd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3utclqhln.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3eoclurpq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3stwfqvmt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lhntubvh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3umpzvugw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mtglmunx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wcdvxpxr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rjctqyty.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wsdqqisv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jiiauyye.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wwunyhqf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tcklwetf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3icfrtthp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jxxtbcmd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dnxdqybn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3legrskhf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mbfpkasp.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlemregx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zkascedk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pzqnpnxj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hoshunjd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3oivojynb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lrcyulgl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jnpuclmo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3udkfobew.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ehfozdrb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vvzhegos.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3zgggxvds.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3gfrhllac.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mkmveadi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ytajwwog.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lbohbclv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mvrfomrk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pqcnglmk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3kxxuljrn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ldcdcsfz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3sqbeckdr.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3nizremto.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vfjhfqjz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3nttontlm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wjjxtloo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3njkxxzfk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3akigpwup.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fgymlbgg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ntefmlgc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3naegvgye.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3apzfrkkf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3nzirscgq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3utfafqwb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3vrcoemvb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cwaqinpq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3axofzxzq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rvmrzsou.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rlgpzzqt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3mrgnqftx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ogrnbsww.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3idmrfwjs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mgdwejmw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lqykzvij.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3rskgriob.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3prhfnuuc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihxkdbcx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmaskjyp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bixqcciv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3tsrvnkjf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3stjycmbg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nxndsgdh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xmyostti.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3uowtrmic.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pxjssadp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ijqxyuqi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fdzmycwp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnzywhds.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rodxqpgh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3edkbfnjn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3egybbuwx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rbvkmsue.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mezkzfss.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3komoehlq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3jtaixofc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3narrbctf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oykfhyza.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mbzqzsgx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hfpvwiea.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfxpgoi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vpbgcwyx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3nfqdaefb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iszcmrfn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kpjiwgcb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3klallwhu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hpudxmgz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fpifqkzq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jdmziyih.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ehmcohca.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fytctxpv.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gqwboprq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3lrjradsc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3sjymomka.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3wgvxtyii.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3uljtgotj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3quomidcn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3eqsyxgft.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mnskubmc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3xritbycs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3agpttdjk.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ahlxttpv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3vwqvxaag.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zfptfjss.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3xcxjdhid.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ihgajzrc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdpjwnyf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3xbsvzblo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qsjmpdfh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vpaenorb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3goujueth.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3knxxycxt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3bgllwwoj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3zuyndzfo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ktblgbho.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zueyqqts.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cdrschsz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fxunmpqp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3abwiomhf.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3qqcrxpou.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3rkzihpel.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ostwhmfz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3womdzgyo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3appvjboc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rhigbsvl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hpliqjpm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dbxgitcj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3hbeaqolt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3vnodmxun.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bpbhogqb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3mgkatsrv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3sdgndhnt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3vdeaqnij.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3rufjxuto.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3knejylhl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wjglgfmq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mftadfdm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3thvjsldx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3khsdvmes.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3nkkgulpx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vzhyetij.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wkxuyzkx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ruswsgqv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ingjxjlw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3mgflevrz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pfedkstg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3heufvylc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kffxfmkj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rnzfkxkj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cdyqapaf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ocwxlovh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3usyjizmd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fohqalls.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xjjomhto.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yypcmhle.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zrkxngyp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3udesgbau.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3grmsrkjl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zakoeekd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxclfs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oxgsvkjj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xhemixpq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ujycbhop.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3onmoeqsw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3cmrmwxww.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3pqoogwwu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3irinpmju.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qgqthjrx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tcumcbeq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3wwxoyhvq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3sbhskrqs.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pmghlsey.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mkhvhbnd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3raeouded.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dttdzedp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3mizouhnu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vwqduzeb.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fdgmjwwb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ofozvsez.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mzqbtvui.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3gurenalj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rgciryso.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yksoxkxk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ixbtcbqg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3piggdxtr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3cfoqxeec.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lvmdkexy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uszurdix.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nzriaedo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3puyakhcb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3filabefw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yuxolost.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fcebmxca.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ydeyjmny.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oiwzejjh.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3scnzqncb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxwwvacx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3shvpvemq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jokpykqk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3krqlyuvz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcagipdz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3sbbffjrr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zmjeoyyj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qtzjujfj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wjtjxcrm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3drrvuqte.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3klhujqnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3slscdwwz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3euvwwglc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhbbfvmy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3rkwtyfyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvtrdcnl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3qslwiecc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vilduzgk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3rnpxssjp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gnrihwej.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iaykjcpi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ogurvqob.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oxeijrqt.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3udordblw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zohmjfph.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3frunqysr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3akcqgzpf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ynucalke.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mmaggwwr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wnpkcrzd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jgltzeou.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3rjbuwlkg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rdrillux.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bstztgqd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xlgghmho.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3xtdnomhp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3uzmliybg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zdognxxo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oxhkujtg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uemjiuoe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wxcaparf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3uumoqggt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3nbacuily.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nqgbsvrl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3klhgswdw.html


<!-- 参考信息 -->