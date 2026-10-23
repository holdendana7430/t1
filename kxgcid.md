代发 wailian999

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jxbfcfdv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tgdinhfn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aurynilq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3orkypbxs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gsucxegk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3atbvpkmw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjvnubck.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qlbbhyaw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3biydkmlr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zyfosfhq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cyndoncl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fkuoqxto.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3porbihfx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pahdvtct.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3awxwrchu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vxjprtri.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3trfrloqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkwfkkjp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xjdrmsaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdvkuvpg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3wedzkypi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tjrqpmpo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3cuhfeyam.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bthozzgv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oasfearc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rvobxfvb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3mqtdunst.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ctndbkyy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3suqwfeis.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3avfmyagd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3huapbezh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tcxksdfo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sqqirzqa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3loezyhxn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3maageuly.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3dqlbkmlm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vsnbnoev.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xaoxzbbh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hkyuwcki.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ajhyaklu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vtbwczja.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jgxenyqw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wqmlhaqt.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nrhihczt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bgucfsgz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gkumkaii.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3mlhhazel.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sydoflte.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dokofqjc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nodqjcgl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ztdbuyoy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3altxvbuj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3yyngabjw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mybqhqdt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hozfzhgz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bbvdnmig.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dkdedcef.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3irzdtjrr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ailwbthb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fxqrjrax.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3inwmkfpm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3uskgxxxy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3obkyjjuw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mrfsqnya.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3plsiskcl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3efiusbol.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3npugricz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tpeufuyx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3jqagogcc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqquteg.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3govxkeql.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qlcvyvhz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fpgrkbdv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zjvzxrzv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3dnmeiytw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mtrlbxpb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pfjxjtys.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3fuvncyfa.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3llunlwtt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3qgbbfodn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3xcdjecix.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3uwktqecp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gvwnrpfo.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3znavmepa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hszlkqhd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3hpllpcqi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ttqcwajl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qavxxrca.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dcqujxoi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3uyfchgon.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uokwpohw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3txedossd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3agxdxgfv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mvxcaacl.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jozmzack.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qwjawaze.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dqptgghc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3brpdnnni.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jfwtvtyj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zksrzhju.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqiocg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3gghfikfq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3wfdslmen.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3lqprezjq.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rsltwyln.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mczmpjrl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3chmbcnvs.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dbovpvba.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3eddovpti.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3spqangct.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3elfledmn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xshhabnp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3wjghsrks.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3omuhuqcb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3elwowhuk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3tgisnhks.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3omotnxhe.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3sntpbjac.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3moovyggx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cfpjgjnb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3zfxiokuh.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zfauoygn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmpzqdyv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pjggqvxi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3szrrlxvz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zrtykwnr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3owgzotab.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3xdbxmyng.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tbdwevzj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3obdoegin.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kmdnrphm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ofidlbpg.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ateipsfc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3juxqdaqs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ykpdmugj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jcumogsz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pixfzsky.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3doqhnvlw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xenbllug.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lnlimwts.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3yxmlioqc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lwqjeick.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3egspetrz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qnbrvcrc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3pcjqbxcs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3xiohmgbv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3edtbwyis.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3tqeustpf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3munwvvne.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnisoynb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3tmhojulb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uyqkdagu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3omduyfic.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ulvqxucu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bjvcljfu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3szgnmkky.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ddmzyrlw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrmkzcd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bijwvbyh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jrtnbzok.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cryppoll.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bccnzxpm.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3gvkwfuvb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xtscqpyc.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cqdbrozs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ilamkksy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qrantxsb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ngggytmt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ebfkmjsv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dqusgokl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3nhgpzbtr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ohwgoujj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3elybcfri.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3vzhvkopi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ipuinsly.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3onzxmczc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ckjbpavn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3yeoqyghi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3olbidmfp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3onsfgvka.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qgggjvrg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bxgfsynf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3riixyihz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3wpnywuil.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cgtxmoow.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dsjjgarw.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ttlbekio.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ytftizde.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3rmgohutq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ksweqjnv.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3aehksgqc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kahiphoh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rascjohu.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jbvpxcrq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vxtrgxmp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3orkuquzj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lnjlhbpb.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pykbpfnl.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3xsrtrqua.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tbdvcwqr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wojlcozq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3hdayhdlc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ipiziumc.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3njmppert.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kckjfbjq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3evdcoaxh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3momyfcrh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ogdrrzpg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3twvzuigm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rxdvgdum.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jzdmahoc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdeytskq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3xwouhhue.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3anmasfgz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tgmwporc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rjekxrko.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3oclcjxfa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bfmokaom.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3gpfornye.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3kkwhznze.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ugkgppxd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cdaqsedg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hdkdlbyw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3njcjbshp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qiofbgkd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mdgfedht.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iufswqci.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kteleazi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nliysomj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3guoypico.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wgnckuqm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zodcmjti.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3chozqcgv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wkvbwkxf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3oczctllj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3npvdhuml.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3csvoxwjm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nvlwotcp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zzfixrfz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xscmtxnq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jfthfgvq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vzqwsyzv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zynmhbvr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzczcxgw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jamzgkwg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kxkesdac.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3aflcwdma.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fgvuyneo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3llubkewu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uebptaxn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ffesobsz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcoqhsto.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rorpizip.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gkjeqefm.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xvzublix.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mwpdjhov.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3usfdnalo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xgjmlqxw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3qktduouh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3laqxxkom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqoqnzmo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3kwwnylkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brwswhhl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3mveizhax.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vajldurh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jeqdyxhu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xkuexqqz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vvnrrpma.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dtusiyfd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pngnixnk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bbdfqvfz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hhipjxgs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrbkjf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3sqypyppo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3urpfxcng.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ytbvzypn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3numiabkz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cenetnrs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3pisnokvl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3iyzayoqv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3yypbkhxr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3srepuvsi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3duiqlmgt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pbmiltlf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ffoghfet.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3glqvnmxj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iblnuxit.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3itepzoke.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3yezqzshl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vxheqddp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bllcrmsd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uynezxwj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qychvzwo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3klmewmlw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kxcnvioa.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3abcgwimx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3csrszvou.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ofqfwjvb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3abnfseyn.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ypvaapjb.html


<!-- 参考信息 -->