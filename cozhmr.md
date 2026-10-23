代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3deeizbos.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wafqntbl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nzqikcki.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tkpccspl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fstdtapp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vxljjbgt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ajjitttt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bsoawowb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tdatuvde.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ielrczqb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxrzwmg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3peubfnjf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cgnxjilh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ryucdvql.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rvsuivxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpvraqxy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3thqhevtq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3afeivrud.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xwzflpnc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3duiibjwb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xauglbns.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kphzoqwm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fkkyrumh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jcjvkwxp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rwtsknnr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pcyggcep.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3cbfmmnlg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hhzpllej.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rhgmcnqy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rpmvhncr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hqzkjxyo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3azdxwxqm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3phrjfdhy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kpoqmlda.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3iqbfcgbc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xzsgdnxu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tzfqnkrd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yufqdqbl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qswxfnrj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gqbnpkit.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zrguzsjh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmirtys.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3egqizajz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnkukmg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dzuuygnd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3oxdgrjaj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3clesmedn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nozpjnae.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3feltetiy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3stkhxswb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ahmkuwyh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dhwtemxu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3etitikmw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3batqsnqy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3nelshgmp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3rffqfght.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bzqvfhdw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gebxpeul.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3dqdfazpy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wkynewwf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlbarqaa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nbjqueku.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fnkzcfsz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lfqsomms.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lhdhmeue.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3pgvjzxfq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bwmmhzkw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rezrlyfr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ymfcztfp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3envfmkli.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3anyfincb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3grnwfhzj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqqvox.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hzcyfiin.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3pfebagyi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3olxwfjva.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ekuphyaz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hmkcmcjd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bkhpjmhv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xsyboppf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cghltfmu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sepsnufl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3tnzdoppl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jiplwsbw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3oorpmvzy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3padplqwt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fqdripuo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3glmwfjlf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3phsskdts.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wyidxxpq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jvdkokyt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3uszhhwfd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rrxsyjdr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ukgbrqug.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kggzzgzv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3omrguydl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wpexpvqb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3auzvvolu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3dparuzah.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhmqeqj.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3udxldzmv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3jlfvocga.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3fbckkpht.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ndkmkpld.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ygtptkhi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hbwfyhlt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ptnucnhx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bybexgzn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3araujprs.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3dpzdvaci.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nxqvrkea.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjksxnoa.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jvxwuyzu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rybeskfj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ecinppnm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cispireq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lldozits.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3kcznzfgr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wzdxkwbl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mtydohdo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3xftchhbe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ryisujyo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3hoagaqqx.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3inynzrfk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jitumonk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zognsctg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3iseaozlv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwcspyln.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nbeooyds.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkjurooo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3alsvwclo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gtyihaie.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lmahvwlt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qwbkmtxj.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aikysyxf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ssocdfly.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3tahttjjr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3schganov.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ybtujfts.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3hfkacnev.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3tnzpcsrn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3udmwaqud.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3sudpzgnr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3uuhtpmvb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hcsazmjl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yddedjbo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mawasbfo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dnxagbeu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ksuklpnl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3mwnphxzn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3rcbrtgwp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gopislot.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3haacpbvo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3eheivqvm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3skiulfgb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ypovhsmu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3huwbvqgn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3txtzhqbg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3ptimjddx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3bqjdfyhx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nekznvkg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mimemsbf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bnishdtg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3rivyhiiv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3viscweuv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fnupaqay.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3rknvqosv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3euafkzpr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3vfltqzmk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ffkgqzqu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kqqiemjk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zorueuhz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mpcztttq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ggadafte.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fsaiamtf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wboyijfs.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3kizvqjjs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ikrhuaug.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gyryzpfx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3aqdarmqb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fgllqlik.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3snilptxr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ooxnsvxi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3ogzcorsb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ullxktsd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3abnulses.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tbhqnjpi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kavmanqo.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3athqwria.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3vvydqear.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3htmiqzeq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmxsaio.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3yttwkpvx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gwyjvpys.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3xevfkqcy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kdlxdlnv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3mwrtmwde.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3aydhkrfi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3flkdmchg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ihuzhqkr.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qujmconj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wisxsqfr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dpcmrkyl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ibfqymsg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3skfosphl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bcpplape.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3aplixjmy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fiuzqcka.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3oqukckwc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ejvcriud.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3muwhaoia.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3iuftpnse.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fxnadipf.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3aaymexwl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3swvhjsei.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3suuojwya.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xyziflah.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xpyogsjx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wkepyqbs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yohybyor.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3dodrgtnd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cqhorcyz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mxdgyevl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dhzsnuae.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3jmxuocco.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mcogcvjw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sslujnsk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3espiuksv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bmjgvhme.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbwtspe.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gynqtjxw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rqgcrrgz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tyrikkqm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3huedemgz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uaqasjnr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fekmhwce.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rizklpei.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cpzufvpx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3vdrexgsu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3azxtvozm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3zdjheauh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3otakatlw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gdpomdkh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgergaog.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3rpxafnvo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yguqmhhi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3mgnxjnvj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quvfybwu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3zrmttlzb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lmowjfdh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ciptncxs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mwulewdz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3kfaianxo.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uxeyeslk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rfvhflsz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3bhyscexn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elsryhol.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3idcouewf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmpvinou.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xetwsspl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3njjfsbyg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xicwttfd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pdrvqdcj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ihfwsade.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3aqnrgfep.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rfttvpog.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dxfkaede.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3kipseprf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3astbrcii.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lgkudfxu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bkgdkcnv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ieakjffg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3cwkvzteh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nucqhvum.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jysymxhc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rvjmuged.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3csfpzflm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iswgkqwz.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ywhjwvof.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3rmvwsigk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsnjpj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3spbejhik.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gdrhdfro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xxbcaqgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nqjtonme.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qhlfojsf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fqqkepjt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lizuqrhs.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ikopaosb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3pccnfhxf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wsuxysjn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wttahvaf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kapjyyjk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3tiwfqwua.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3tdbquyft.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lqmvyisx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ckaoxjpx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3trazpiob.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ysrgmgou.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qmbmijny.html


<!-- 参考信息 -->