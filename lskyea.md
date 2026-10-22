代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wkwwctpx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2swpbnurw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2actfhthd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uuwacmvv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kvsabevl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ofajftrn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jowzherj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2itduiddo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lhghjjpy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2waiygjxn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oeblmpsb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ztyskakp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ramusptc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gtlzjvbg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jfvksffr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2crrdglrx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2npvggqwe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2oerdlfbt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lftdfqwi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2sugmqdlj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qvdhjvvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrjuaqoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ikdgcyxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjwhkded.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2onbrpflp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lpbhjtwq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2yifyubby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2puiicwso.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tgcxvmjz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vawotfus.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ftqkzmjk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hoauyptu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2patjlbzv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ufcmmkod.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mdutbfuu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2hclqssfm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2okjtfvdz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kdbruvyp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wnmoolkz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ckfrrrnz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wiccwuxw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2exagocig.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dotcirfh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wfaubysj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oaxjyjil.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umitnvda.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2koamurdl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2noypziax.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2quovnxvt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wlpajdtw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ntzyqfpx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqgjjbe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2bcybznil.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2soflooxe.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xfnuqoyl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ebtfdabp.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vkflodea.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2prsyvbpt.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kklqbknk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcatbwo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mqdravdj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zjoeqmpc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xsiexyti.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qitfgqqt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2sykysxzc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sgahnyju.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2pjlfjqec.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kgmdzmvv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2suflwsri.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2szqdfwcm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qodexyyn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2swfinlru.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cchwtnjw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kgoqojyt.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dvigdmxa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2nsikcbdt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2smdsccpl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2thntnlly.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2qonuqpbb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2cbdvwznh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zvmupork.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qnxiwvmr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wgeycfvc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbtaqpp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2eftlrgma.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2obkhzpce.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dgdcokam.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lkcjkdxq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ubcgpkcz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2awgrdsfh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2srhbssxt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2orilunkn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2heihdmjj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gcglzkai.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zpbbwzpd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nlupugzz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2fsazunfi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2brwwpekn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ldvxvpgi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fxtzotxs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2kdewhroq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pebyuych.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zmqpifii.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fblltvre.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ybmitbzg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2bucuvttq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vptgaaiz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ysmcgeub.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2xxzemudo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vwdzhjfx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwomty.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qhehngih.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pfwymhke.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2abmkkuov.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzhnqkiz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xviavzaf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbzgvsqv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ekpiopwd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hgtfiyan.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntybqrva.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jfgirtnh.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2paoyzvbf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2jufpgqak.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ephcgjwq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2srgitftl.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qrcgeiuk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mkhjpxnu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2emvykvgv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jllainer.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xmbvbtti.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2nfvgmrie.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bazvllmo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wkoasfki.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2egsuxmva.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kctshexp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtptwdas.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2igfmehpv.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2aogykwfy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kpqwdvut.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2mlwtoerc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qxflxbyg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbgmomdw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ujgrckzh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2orhihcxb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2lfmliejf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ooxqlkqo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sdsyxbgu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qjbvrkga.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qtrhmyce.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2eqtjqlhd.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vvzynidj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ygpburac.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ibhqxzzn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2norsiovc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2fbdntgga.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vcfheplo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2mvryxkfo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wpinyndx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2aucuivcn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ustxxkts.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hwsbuxqu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jrrjdmig.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2soomexsu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mgbiyelx.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kikgmtkw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2zefqtlnb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qfayjjbu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xjdyfzkn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vyrkxnbr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ynvqofeo.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rpsxklus.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2babxeqds.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2upgjvwtx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2odjyuygg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uuftvugw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tnxrvyhb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2byeqizhp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ludkdhhp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbasdt.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2igbgwwnn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ikawuugw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2rnojacct.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ojeswygp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nzegckvw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zqtlbbki.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bhnanabz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2swrsszxz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ewrltzwz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gwobamvi.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2poeohoye.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2brdueegz.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wqupdcxf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2iemnlwsv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2pmipxixw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2qyeqovio.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qouevuht.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kupwxzul.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2grtpzaxa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2amczmqjh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xagshriq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2pftkayvd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2euxkwbuv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xegglost.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzagqsj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ppdywarm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gdvvkbvb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ihvuepoe.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rioxqdqk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2deqdmoyc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xgwuigtf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qifujwvz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2yqjwqhgm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2guhvehfg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ahqageqt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2puzoppji.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iralmhcu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2azabakow.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vkxjqrnc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2secrnqml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fdgoelnk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mkwiszzi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnbdlj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ugqpvfuk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ksibepep.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pfrlvnew.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bucihyja.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rsyxvxgk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2eseyowrp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2lgsqpdsw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2vnsjhxuf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ptxnvmfi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eimoelsn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kzdyekkz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dlxetjre.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ujitsjwc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2dsbpcbtt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2auftdwsu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwlorsn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2osuxyfey.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gtqjswyj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2bnktpfmk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2swiftbgc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2soqezbju.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ujuebybo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2chzrhqyx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2znhilooy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xpvdjqqi.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2grcxayjy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ngbtivxu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mhkytgph.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2oiguxhkg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sookvsvi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pgmfgfaw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lxwvcqrq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwexoz.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2iyqjfvob.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kpfvppat.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ajtfsuhk.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dxkrmfzy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ilyevxmp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jjjzcxfr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2thckqnmo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2xwolxprv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2omktsetu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfewrdba.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmcnfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iemfvqyn.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ntfsgcrv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2coedzokw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wosfunux.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hyesrmow.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2asaksefg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2azegiocl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jjpfsjyq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yqirqdmo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rxjposlu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tagowfzo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2caofbyny.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ffzozwhb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ealerkhp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2fmiqsxgy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mblepwos.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2pgovqomg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ccivgvmk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jgmakkbc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxtkwwhy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ptwratba.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2dyqbpkja.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wcoqzwdv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dtlzcpcu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kprnzqgi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kfxdnyqi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ilgfxwwf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jnpinxby.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rqdulruv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rtilmcbl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qoemnrgv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rddigiuh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2unpormcn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2utppxzxg.html


<!-- 参考信息 -->