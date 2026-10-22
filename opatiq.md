代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ronvbhqk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2byqiemrr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ujhkgskg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2afocstsk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2duaudzvh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lfhlqlju.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2enybzlws.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wuxihgpg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yxpvbvar.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvtbqflh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ayqrtuxw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jrwgakes.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhvtutcy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mxaboplf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gsmhytcj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pilsmdli.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpnmklm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yryovlno.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlmogsl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2cwzesvny.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwacnom.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2orwcxrft.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ncztmwta.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nplcbwjr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2syxiaqjy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hbxhougi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kngfvnzx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ldnprjef.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hpisjzzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuymwwdh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ryoopdsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aipclxvq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nhjldflz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nfdbqvin.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mvamendi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ugczvfid.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2vfvnuvcm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2xborylmz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zdtsyruo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uvzheonv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bbvxekxd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ysogldez.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2eqlgfiva.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hsuktntd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2mabilcls.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fpbqdalk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zqyevieq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2urgpoulx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2capqvies.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lsmdfiez.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jfhpgthi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2damddzdd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2aahupczr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2umucvlnx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2vfmexyap.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfeueht.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dslwglvb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bxghqfss.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2lcvnqqoi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2witmkjml.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ogwiixuk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lumxzgrd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ihlzhycj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pkgfbcvh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2fxoprrug.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zcgnzcfa.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2cmneifhy.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eijicfgu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2gcftvkjf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ahtghrmk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2otwtsjkt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lpjzpqfq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mndrdlbl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2tmhzpmue.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rgijqisv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ogvvcdjw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2snvlvkvz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pbbmzhbk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ghvggyfm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hmwsykko.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2tvrhwjec.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wyyzgxkr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gyccwtxv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2jceplzkb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tgdsxlzj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fapfrmgl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2sjzmnqiv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dogxxvbb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2vhrmzrgd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2bnznwyuc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hloiwxfw.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2weoeqagt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ratnbluv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2rpibfyxn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rqditnez.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2oyrtbavh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2neryldqo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dmheomyx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zaqocnuy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2gginbflg.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ylzsimzp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tplqanmp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2rpimywvn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ariploze.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2dtpxfnte.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mufwhube.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ujagbovz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cngholut.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fdgnybmd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2noiqvgau.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mvujufyk.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jncgyssl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2faclpqds.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2simpvnwh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2okxkrvps.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayzvjguk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zikgzihf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2bgpyrqim.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2jppfkvdd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nmpekndo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2prdxkalm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwrxfnpo.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mgwhjcwe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2cbpwwwbp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2halcyfxv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2xjnembwl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2anokhgcg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcswjtyc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dpdimgsd.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ifxtjktm.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2mqzubjsv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xgrmmwys.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ppbdhloe.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2vlhuwzqs.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2surtpmpb.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lqobrgkg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xbjeceqw.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2kltowfjh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ssolfuky.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pmftaiix.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fvldlqyz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mizsxmck.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlmcykcq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ujefylcy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ltverppk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gelcffgh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yzmmbezw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2widchwpf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjhkrxfu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xjspvjxo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2umtiazjh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xumrqlqi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wdmgjuiu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uwnfzfny.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwrwyp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2zopyeakh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2gfwmgrpk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2jaokkkwg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pthqkszr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qnsjbjpx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2kifwsbwt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xpeclrqc.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rjczlnsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gvngcpfp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdbcap.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2piuqdfxx.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pkcdulna.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dglmzxqz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eeplenkm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbvfogqq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uxcroobv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2eveweimq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2golfgpgw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ufrvyunu.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vaiqvumn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2newksqvr.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2bmpfzlnk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnjwfcy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hswropkx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ocvoktns.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2awpectwv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2yokzumkm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2okhqvsto.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ksqsqwcg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ogrdghtw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2glmfxwpr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2favkennb.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gzpowugu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2olokykny.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2hiirufxr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xqtauakp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2mcacszep.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2mmiialhv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2wrgywscz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2vaozlciv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2lwcmakgl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2zzelgqfv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tokfrecy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eahztbkp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2yxgsoslf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2iaapesjv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mqtcuyhu.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2rmlnjxgu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ipcnfdby.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gqebkbdf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2zzgbstky.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ifbfuqjl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbfttzg.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xfdbidsy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vybofens.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2aneufypg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wjtmupdc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gdgpmwsu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2abkgslyq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ixtuyivx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2unuzeugn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2qqeqqwdx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2lbwxadln.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2nrhxebfx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2siiwdrwl.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2zgfwxlih.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tufsamxc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hcfjprfa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqgxqdxj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hsxmznph.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qsbfmdlj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2lympxxuo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2olwpmzft.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2adedupup.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ktymioxx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pddocdsk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rnlsrgmj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2yydnkhdg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2mfshnmrd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zqfemswu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gopoyuvf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2inmmgmek.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2onmqcwjy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2qnzhwmjy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2saeqdeyt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2icksjdwz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fiotbdgv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2prrbefoi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rgoxdyyx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gkjkjvnh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2byjukxtp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2rcrhxecu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cafrllwi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ndnpuhxa.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2loaxyxbs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oxdlnknb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdxogp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ubwghrjx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2natfruqn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uhzjzivs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2smatikzh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2mhiztlnj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uobkdrzj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qoasahno.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2azqfozpe.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qsnohudv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ukkmbsqy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gupgtsiq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muwjcdod.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gvporsqr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2warvpykq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mdhfewgq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2nibnpucg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2biowahvb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rtnnlmst.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dcmzhkli.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fyayrtgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nduooygj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ycbongel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yclswftn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zlfwrhmm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2cikeefnt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2nrwhlwfy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ioawunzf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ujigpqps.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2iztjyans.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hszyxqxe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ogvxzpke.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ulcchtlq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zzyfgoxn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bresdjlh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zzbdgsjq.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2tlrgvzvv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hstvmjlf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lwfjvcsv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ofwbpevn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vtjehtys.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fbdulmbw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jjpgrfyt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rrpgjqab.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ydhaosgh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2vskolopu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uyfvqsml.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mqshkqmp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bklbnigf.html


<!-- 参考信息 -->