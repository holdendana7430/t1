代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iozyxgwt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fwtomamu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ugyccfey.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rqborfaz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3agarfzwv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3urzwpxfi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ajukustw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rrhdtxnw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ncspfebg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3odjtigwm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tfuodnfl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qmovfjcn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pwmfqzly.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wstptwzi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3csuxktxs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3shcblfaj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jvhvljxq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tyoqyugj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxslvey.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3evlgxagj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtzqvwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnzoclsa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ktjlozxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfiuyiwu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dhfdbvxh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3crloxyua.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zjbyybjm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xjxlbxgy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3vawmilpa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fnkqbsec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oijeriax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3lrpaikxi.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xicefiee.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xevvvlqi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xsdszpta.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3apmuixzk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jvhxbgnm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vvwvrczx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ojtofopr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3fzskqgge.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3giwlyjry.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ohrdhrqs.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wibkyjhm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3saszophh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wqfwrwgf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cvolfrng.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qvkdwupb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3limhkwlq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hsuysxtb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kbvlxxvv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3eqlyufkm.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxmxhdj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3oomakrxh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3skgphmye.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fgelyhqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3abhedqbw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xbucygiz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3uqxcjsma.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nkyjarbi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvzdtqp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pnwcndkb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hpslvecv.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3rooxpgpc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3iktoycob.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3fydxojnq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3eiskyorz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3twozlcfl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3brcdkzdk.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjvgfija.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3whdkuedh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3dpzjhylg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuuhxqb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxlthj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3fdshqdgq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3fgwgwvtu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3sfabbcwv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mqytgsfn.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3gbrdqlez.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xewkktde.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tcmftvze.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cprgiofx.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3qthjiuhx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3putpqfhb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbnodst.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3vujamtff.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cajqipmw.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nesgqmke.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3gercebax.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qincxdok.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3tjextkda.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3kwvoszwn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbwsfnl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3dhqzcnfo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rdcvjynk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3riupiqtb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3avledvko.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3qftysdim.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3aeefdmmf.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3oylkxfxk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3decvkwqz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3utoggenq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mxkznigk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zqbnwsnr.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrnypgy.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3gkjcxfad.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3aozrazou.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zpedgpfw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqacwxlt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3holookkt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vbyubgiz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3avxphgjh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wohesfos.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3uiutzauf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rdaodrec.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ishbojtc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3nqzlijym.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3plomtgwa.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rrzrrvdv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3wvnngqvi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gvgicgnt.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3vdqdaghl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3jvluqozj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jksxpxmp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wscgyrvb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rwqhdhbq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3uyynyidd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tpygkorm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gxplqzjo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3oafcesxw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3xixtkipf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sdjczarg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3fboanqxl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3oqbsudyq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zdrvnvhq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxgszfvr.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3weqelabd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cqnssjyf.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ionbywyt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3sraepfzy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3ngsfenll.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nmgswrpw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yflopsci.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bvskzenw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3kjyyddew.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3fjmiusuu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mjudjgdq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zcyvvznf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3suojdbdp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ypvtbvzc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqaeree.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3alrxhsyv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3unybdvjj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nyltyvfc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mpphimhz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yceuwsjx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ajsnecpq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kdgjgoyc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3xeupoost.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fyxaqosf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gtdwgqry.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3efqcqocd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3awakgtdo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3quudelib.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3rglyvcxo.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kffxtuqd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gwhzfuxc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lkybxjbs.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3evxnwzik.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hgvlgucq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gnnotzvw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lmhrtcnf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3robnmjji.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3jslvjjeu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3iuemliuo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3cstkputk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3cbmhaglq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3cnohkghb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3sytdrnax.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wvlvxbfw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mxcpxmmg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3knlvgmnl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3vkpkztsm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3pkcinqnh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ktodobjm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mpshgwze.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jmnphypa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3bernmlwt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3rgpugdul.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kjrgtsbx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dkvmcrdt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xxttkarf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jyaxvpvu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ztiditfh.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ljfgnbeo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jdcfjjbz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3onemtxdh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yppfqloh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ipvjhtwi.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3pfejruqc.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3tummsupa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qawixmhr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntfbqygr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3otzmcnea.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3otlodjcb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gxhkojvr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tmercucl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3shkheqcp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ubfcycow.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zzlswfru.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3djwonuyt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqffbitx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rtlaoepq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ptrlsoeu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3eenreczt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gfijehyj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjmzszh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3perzdgdg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xvtuauvv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hfryrlxu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wtvewsdb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3kocurtmy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bxnxidad.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3awfvrdfp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3qbtjcmdc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3aofzbjlo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rmextvpt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3nxgqmfco.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3puazgecs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hoqtmkmv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3izcyjzol.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3equsptuz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eoqhrfkg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ujchcxfe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3evwxbsur.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fvotqema.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ojigmquj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wjjlxewo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vmahjnas.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3kctshexn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3erjyiqgx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lujhrjju.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vwaxlxtv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qwkjbtfy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3izlfraja.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bueeuioo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kleoydme.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3emyutegd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3agqnpyuy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nyqmyucu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qgrkwcqu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3oataswjw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbatzurx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3exmrcolp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xvdgbrpj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3evikehbg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgrlxc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3biasjwtp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3cujbvdid.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3rfvynmiv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zkubhfnw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3obrvoefe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3siivnppc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jysislzn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3owfcuokz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akofptix.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pgjslqih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpqyefvg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nyvampxx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bgnbbxyu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3msxaktat.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3axvsasuu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wqktgcks.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3arkdwmiv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3noleshhg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nymxbqre.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jazcazws.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lauayjrk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3etnbgonr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3enxnismx.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nfkilaon.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xecjzbgj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xtfkximg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uvifcwkk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3nwuolgld.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pmzfumgq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hlmhmeuv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dwsiogbv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nkydhnlf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kcfyvyuu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vxwdosij.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yjghbsnc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rgwtwcjo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3hkdxvxbw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3wgbghadh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3inyzlfsk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3apspomkt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fxiojipi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3durjlhih.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3egrtydlt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kcvegref.html


<!-- 参考信息 -->