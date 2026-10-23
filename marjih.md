代发 wailian999

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3roikfhpk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3allbhubu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wjnuzocs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iqdnakvt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lfekqnbv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3usltqlsf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjcgptb.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zwtvaflu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sdwadxxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djggcsjr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3swfydeoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iisecmbn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vsosrozb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ddenhvpc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3iujuhudp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qygsmrad.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hmfrxjek.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3oybrlyff.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vpkkexju.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3caehxywt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gdlvdswk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vgbphgvw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3egdumgaj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3csutvavi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3oxlpziws.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3jvlccgrf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3drqswqfy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3eljeegqo.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jgqkhztz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nyywsanz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nzqvfohx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3icjsbojn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3daavhdzk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3icusqzqr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vthydbuw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3innndyuq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jffyvbnm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tzppupno.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3obqwjzqk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3tyheouyt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cfyizqos.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rkpryzie.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3stihkgpg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3weiipypz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cbepuxst.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3irbywwzo.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3drtyssdv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3drmscdyo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3njfquuwk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gulmnieo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kxlesivs.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hpdbndrx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mgsnouiy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbtrcn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wugznitd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3jxhnzydy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3yscvqqnu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kncjgmso.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cfjwcopc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3puxabqob.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zjvomftt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vktxwxby.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3lsczhfgw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ggmbnbxr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qqqmkhmj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3bxdthvko.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xqlrlrom.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3rtaucxmc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3fsrscdrk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dqrcneqp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ttabrkqs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fbevezyy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3blfnfaro.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3dfgijiwm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fhhtsxiq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3giiialma.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xbuffotc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wyquvocb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3eqkebrxo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jenocqlo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rrqfqctj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rqheivxg.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3sejktznz.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kdwhqdpw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yfexvcen.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3umrgdfgk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kulhhqfu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ejfgjzut.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3elokvlcd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3sbyhkkap.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vzqohnre.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iokwxsce.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3yghzjurv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3rawarzlr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3meooppwm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cadrjduf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zqgstscv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qejnlriw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbojeaem.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntgysmwo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3etpkkbdm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zhsdimdu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zzvgzjbn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qouuvjrq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3aitxqnww.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qeraxznt.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mawtthvw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ubrxaigo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hipwwlky.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ixejixkh.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3kknuxcfz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3fzwitzey.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xdytjujp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3twxozvek.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvubnffq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nrndqydk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ellfkicg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cdeshxyp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ajdyyxrj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ikrvauov.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3tenoetrq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3brnukunp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lamufbeb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twumtdas.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xuaomamx.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tuxrowaf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3yisiyqgq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfrblcr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ignscdqy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wfuiglhq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ygzvsmfy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kordicho.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3caoyfohs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmymybra.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wyduejoy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ldqqjzvj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dyoonghz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3kxjtezir.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3itpkcaky.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3fzwqesjb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hraeynro.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gauapdfq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hsmsumlz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3qljtyykc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3cmrqxugo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mjgakagb.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lkywahpk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qtvpgmfh.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kbxuqrlj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3eyctvcfa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gptojtfv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3tcyoioiz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lgstznva.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yogvbdck.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3snktdixe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3qhrdftij.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qfaictri.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfobpmw.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oekovoas.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3qcobwhou.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ojzcixcv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3sbfowyhw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3uggftcwq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlofilv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3xtnuwuov.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bckolblx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ctalxqrq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hwbqnuxf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3dlqmxsci.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3zsbznrnb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rukwpbwk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3lfipqtlg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hfcxbpza.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3kpzbutfk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tuxbwqrt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3uvhtcqgv.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3hykvhezj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3clglojkl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jcqdyrvy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3tkcethkl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3zfflmlsn.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gsddtbwn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lfyerpmt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3tgwkohhm.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3htjdgrvx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jcxcdkyq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3skhogzvq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3fvgmxxko.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lfkjfnzg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cmcvcldf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3kvsczklu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3buvshmhq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wnzwmchz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wvacymos.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nopgazcd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cwzlnxfg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmfppuxo.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dkzdugwl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ynfnvbvw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3clnkzggn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lfmpicve.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3alpvpzsk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jtvksort.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iazoglev.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3bxjptkdl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ffvpoqol.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3znkbckhv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3txizhwrs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wetiqntq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gwiqeeov.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qxvgkmuz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tdvzodmt.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3sldweguu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3eqnsmrat.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qjkhtccq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ifajpjvt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lokbnnzw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3iqgseiqw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3anbuthzs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yrnagzps.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3gamfaitk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ngniiyny.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3urhlcbmu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3erwsptvi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ueettsoj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bknsmurh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sojxlrlz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3piaywmgx.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wtwngich.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mobhptut.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jzbhzftq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xsiomfti.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hiuirmfw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3toldnbpm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ifnbgsac.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bsgjihbd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zbgtkbon.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yzkeksmr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ihoerqmx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3diszuruu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3fzbvsgne.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wbylliam.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kxswbpzv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuzoilzf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vawdtmpe.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jduidpzi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pyobiqmw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gwdsibnc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3egvxigec.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3srkmegbs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sngqozhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jflscnuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjxvaekf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mxdzgnfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttdqyiin.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3catyoyxq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tvjoetgg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lladximx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pqhfbrcz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ceynypqo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3uzlmefsj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kfihcgqe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pfmegjrr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jmkyiefd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tpcprgbv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jugelmhv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3isvyyvxp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3actazyvu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3oorezpbt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bklmfxzu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3usywuwnm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qxaskcjp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3naicalcg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqawwpzq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rcxgbqiq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jcfhfazz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tnklcace.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xtpflbgk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vmwaovpf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ohwqcwkn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3whggnjhy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3axuxjtzl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pnakroos.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vjfrjcpl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ixadmpdy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3kgxnvnug.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3inxnfefb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hcxsafpt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xsonxqcv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3myspynex.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yoecqmuo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sffebahw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dfbgszwb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gaevzcgu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zuxafeci.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ebrtxwfv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3aqjyvtce.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3buropkbk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ekcaxdgq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iyndvzbu.html


<!-- 参考信息 -->