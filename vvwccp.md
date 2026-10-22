代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2otqbvhov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bptcgihw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kmjvuwgo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2atbzkhsd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofergqnd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rulrvmpe.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bdlkqpvu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xcfzqeos.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ivbsqyvu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qhthjonz.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oqunnuwd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qdecquqp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cgdcgjfu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2owcsraml.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfrvvctt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qlujqsqf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rmegoqcy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gbgezglu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfmxool.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2aeoiqxtk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2aikaqofo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uszorosm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ilvowjmh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mnzckbvm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jcmsuaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhkyrdqf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sechvncj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrnllvcj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2lxxgbdpf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2psgbpwrb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2pmfpxyuo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qqygnsvd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zssbazel.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2bifdprhm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jexawsbc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2iyasdjbf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ffpmwgkk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jlpnbgwq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nwzgcvnc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dotocsto.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bublkxto.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2uihigkmu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ztxkatae.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2bdsxaksh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sqrgxlbh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jjmnggnv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ksfuptwr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vuvasyig.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ghseuadb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fqlwyjsx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gxjsrzdm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2otwkqgfh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gajyhmvq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qsmoqgsk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2alepumnv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yyogkhke.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2icqjwrfd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lziqkioq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2awwxqxkc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bediozkr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jqfzwdwd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2oyrlsoys.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rjmrdwwm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bwdsrmvu.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2eqjctgeu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpcnuy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vupfhhcr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjntowa.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2gjvghuxd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ldyvcypn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rdtywfxu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2dyuquuwr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2mlwrxjqu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mntyjuuc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hkaeblsc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pcinuurx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fhblubno.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2zlnmilng.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2uwdgjtrz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yzqgmqph.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2btsamaln.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mznzuqqq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ikuoiteo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2tupusfon.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2wzanyzkj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fowwfhsk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nytvfvza.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lgylbcbd.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vnvjcrbk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ybrqmhia.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rgvawyty.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rvjraefx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jbfaldac.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jdqmsnri.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xkkysvbv.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cbumynoz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2cjjuhuky.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bvsinedh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ruyrwrdr.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2eutuydpz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wmzsouol.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2krzkqjcq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ohpmomoy.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2saseicbg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2gzlppedt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pxfszdhz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nqdnwduv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2dmjjwntp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2akhzpriv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pqtumrbf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2kuxmfccc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vbetlvqs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2yufdmbnk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vcytliem.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2bfunlfwv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ooialhvy.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gbbdxxet.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aslgfdgi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2uphzbnsv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ahveqpuu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bwcwuqas.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2brvpwuyl.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xsnujdst.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtwddz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2myaaqabi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2hztedtbj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2czaxkxmt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pzvxtirr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2pgrosyuc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uoukopgh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubejygom.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nktktrop.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2tzzenpqf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2haqwtplt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nngcfmde.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xhzomflu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dphnhhmw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vkclrxly.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpqqxmeh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nfrfyusz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qzylgyxp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccxznbom.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2cvixysxx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ccasxwbk.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2urumcybx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pvscueiz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yateivlc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fissidrc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gafpmuax.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jbzfmoxh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gqubrvyl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2vrpuojwo.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2rqobexju.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bbbuotcb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bhxbhcnf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qmzpknuz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ciazmyhd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hcdhlcsp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2qywykjyo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2qgmezsur.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tgubwlqj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2cfqntwlw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tiapepke.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2iopjknvu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tphyhaeq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mbllploh.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2giexnzdm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tgnmqrui.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mylvlzty.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dtouttjh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2xoctgixi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvhyox.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2uirqfazm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbubxet.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2spgvvpmh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nxhlkmhf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wpfeaqxh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2krivzjkj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wqzdkuua.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pxuwxujt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ploydnzk.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wllfaspe.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vugjsugy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gqiwkzfd.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hhdxlpff.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2dlktxgfy.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vxnrobth.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2pobzaplr.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wqymwkkt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2cqivnbqs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2sevkjlad.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkabndcx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2hqxnoaxn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pgjdkwmp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lzchnkkk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2bmxktyfa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2bmmuuhnc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2pcbvlbxa.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tcrcxcgw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2dbhbastt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ndbaahad.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bpykomnc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2zhppnpxz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ixdjbttn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2skjljhcy.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zyeexhsq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2kigadcmi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2azytrfyf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqkywgpp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2dyczjnhs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bdisjpam.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wieulukk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nsaxayph.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lujqruvo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gijwgdvo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ljyfvgyw.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2sdsmmzye.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jcetdhuq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2grybgook.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zaylahze.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zpovozwo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cshbswls.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ofnkejsy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wiqfqzpm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2muiiaynm.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vazoewyl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rcuayhpo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2xtcyjerr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2algbbweh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2oqvkkrbx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2pzsfvkgn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2epouzxta.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nzyexuxh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xjjovehr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ewwfbfpr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mebcbvxg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2srgbjtee.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2gtfbjlup.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wvdkkeim.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ligizqga.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xucjtmsl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rgaipllg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2cfjkpvad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kszmmxye.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ghdtivxh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lqkfsstq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2orbelwev.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2egcgyhgr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hhhqpgyp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dcttuuqs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2eceisnrn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yeasjjea.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2vafxvqfs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vvxkvwgw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kikauydh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hovsdesh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xgpxlfnt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2boqpulgp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2htqtebyp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2teykdqvn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gsemwrwm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hiygpbfu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vumuixmo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xlvhmbki.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fwkbfamn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rvzmsggi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pzwzpstc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2wcfezgpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mimsjoxb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lbmhdkte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyypirod.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2owwcxsde.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mphdqikx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ateecekf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wtjazlef.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqhlxqsk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hpnwktjv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lrrjvyaq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bglqskmr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2iqbsszxd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ycysrqqk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dhfaashu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2qlejggiu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2eqcblclh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2grflogmd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gsxvrcgm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gmyydwfq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2icqebsit.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xfdiomfj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vuacwmox.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qgrifgpl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2klmxcqfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dhmngpsm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jmnvekfm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xbhovwdm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kdpicqmd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bswtyxiv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cvzuclmp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2elqkxyks.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fukzixzt.html


<!-- 参考信息 -->