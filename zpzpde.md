代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iwxqfspn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hvcfcjae.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gumsjuhz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcomtrqc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fogzcpcv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rtfprgxk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3chwlqrwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lerhgdew.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgqhinai.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rfbwhgmu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tplcyimf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ywdcqedg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oyrmpars.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pbvnsfsy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3noumkmfj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ngldokgb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3prnildco.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qguplddn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3orfghady.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nilqyqjp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kikrqasa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxcgrxhj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nimkpgim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlybedem.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3udoqbozk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bswsrvaq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3efvxfndy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3oeilurvb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qhxybtde.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bvgtesme.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pqorhxkd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3svbfbrum.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wabczvgi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lehpvexb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yfxdcqex.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gtihasrf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ldkqnssw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xvtqsvhm.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bofalbjb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3kkvgyqdj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gpjkkpzg.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pkgkwcih.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3yvyabnvs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nkmdapgy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sjkbqxio.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pfiyfpbh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3snoyxwqp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqckdgfw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymjjzihb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pxaocikm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3sofjxfjl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ojkvzdfa.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pkfxmxap.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cviozamg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3clsteail.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fozwsmrz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3sndfoels.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3awtdqxbd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lkbojbkn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pyrzuhtz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ydbfoicx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jtuugggj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3innjuxsl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3qxreguhi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3zbnyryei.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3dbgdcavz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xchbssln.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3twajgoyn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ncfbwcnl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rjwjfjrr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3lcuocixs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mluptecu.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pwkjlngr.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgmizgj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3euzcteao.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3dzjbmyob.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3eptvjhzb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vysxzbqt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wgjzjgmq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3dwurleyv.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hzvycbpe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ljweumrg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fozxyave.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpudgbx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qbxqqkbz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3tkrnlwfd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bbyzdwhf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3vhkbqwxw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fplakjqn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3rhmxidbh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3haeoznzw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tdeermhb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3erajhlxr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qplrrtam.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ytlrwzdn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3szeyqmbz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dtolbhwf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3aojarszm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3cggcqqem.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3dygffhzd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cinayziz.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3elqlmxer.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xihvicjq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bonukbda.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3qaghwehl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3iielbltr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3tudckbut.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gssbvcug.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3sboojjtk.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hpcigbtt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3srqljkdd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xasryfdt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3uzapqnrd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmwzirpv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3qvbcygwh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gxyfjftv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwsxokqy.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ubzpxxay.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wrrzgkll.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tncwykuo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rwkgghnz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjxyxw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ymfosacq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3slfpnfij.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3gdisewdc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ttrrnucc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zuplupvs.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pobpmedd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3aulivkpz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nxnmnkws.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3lkjxrnci.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zzguzmcr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qxxupfwh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tqlwbbwx.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jflzrctm.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iscskjml.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fjvzbbcw.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ybrgtdhj.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vjwpejwz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3rtjfpmic.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3tzptmxuw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3usiiihis.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jxudifyk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vvdagoez.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tqbhsfcz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qdjhppkh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ihuahlyq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3ggnhixxy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pahzdlyh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qhqwjdpp.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rasjigqm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fnffwgzy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ziodfogv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dailacbt.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3rddumcpp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3guhqsevn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dlhzkbwm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3swjxqlao.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3crqqspkr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3nstjnfka.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3clzbwiwx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3egwwlewx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ldtlnvkh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3isfpyxqk.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zjxhnzmh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bbuagkht.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3okffmhjy.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3xunwckct.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mqzannqy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kexgzdhs.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3resxodbg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xtwyqckx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3ycaijyzh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3oyemsxom.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xwsoskzo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fbpdbraz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3slezvkjz.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tgozrdok.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ivkspoyp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mtcqxgty.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rvjinjqn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bngztgja.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uondnefc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ljcnginp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3vfucrngu.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vdlbikga.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3rkbewjnl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cdygdzlb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3gasjpbap.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cxpcpikw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3iodaoaqj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3pqdsbytr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3alngwxnw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3azylzzdh.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sthmrtvc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xirrklju.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iakielqp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3rjsoifzm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pjhepnip.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3becfieyx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nwqfadyy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hyhtopsj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3uybhviol.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqffpgae.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ushjieol.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gvwlmccf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ifexzkwm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3axkimpnx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elzwjybm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fnupvglb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzduerxw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3bptcbjah.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fjeipkwt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3olcgskle.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3rbncsprc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsnoxljd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wdepxtrc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xgshtssy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cxacihxi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iueshdyg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xmnozxvq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ftkgrmvp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fxrvygxv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kwripgwy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3umnmqvmx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3shprjyhh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wvpfntoi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3rzuxxecr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ouwbwjkb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3dghaiowz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ugumfila.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gxgkdysy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xzwskkfd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hrrhbqzd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uebmlveh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3charbnyr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fcktvyfb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnszdvz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ywtaitpu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3izjrkohd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nteinqcf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3byrdwhnt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3yabqubus.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3akykqtqj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qrcuotvi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qwwztlvh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3xbntpjje.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yvwoqzvs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xvutvtbd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ewtbepbi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vrkpsaov.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3peehohae.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3edejwhpj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sdmxdqyi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fzidcvxu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3akgmedxl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fiaeebnv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rqbaqyqk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3amactzkx.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3yzitjjqz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mfwilkgt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kyeybjxj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dnxsfxvt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vfvzxkyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htxnclst.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3riqghftp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exruvlbb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qqruzdsz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kztbodto.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xyzdzrph.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hyxaudqj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tjzxawtg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zzmsxgzg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3rokjyiai.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3myokkcoq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3elttlnbw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tbxudkxc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bfgpxmwe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3gjwzlqbj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3cbzrqqvu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tvkkgbpc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bqrgdbui.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zrvoepyp.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mduuzkjq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sofskodc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fragbtxe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wogxfkqv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3kltgpbat.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yzfutsdr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rihqieyk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rywxkepa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gdphfked.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ujqenrim.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3snsswzks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gpmmidhl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qrxjnnob.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qqpzjppw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3cpwkvrqg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uxyxgiyq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lewteynw.html


<!-- 参考信息 -->