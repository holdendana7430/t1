代发 wailian999

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kwatvazz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2drwejxwy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wbzuccwt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yxsohlem.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2opynisjm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2urwqmwim.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmpwvvw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2lgihldpe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tdyyccqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kafnolke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mfgncmvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cudchgii.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bgrcuspl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2alswkzmx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2kspiodxc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iyrmppha.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cjilnwkp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nnbkyroj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pvooovmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2akcecfhd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rvlxzvxm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khodhwpv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2soqpwtmx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2aaaegxdm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jgapfwzs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uamalgqq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yvzcmxfv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2izrggyrl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lweqdkst.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2esjaatqd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2oocslzqx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2btzujxmw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2rithumfd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnelwck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ryseyqtm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzccrgdk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vtqvvaiz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2kdanlkbx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bijoubxk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2trafoodc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ovdosypc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iathqraf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wczokrgy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mtbsfjcr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wsgksmjq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qbnfcxxw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tpyivjev.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ehdcscpn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mteqjyif.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xujymxgt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2tovjqfma.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhzjtdz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2sveyhvnf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2yhxabrjv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2upetpuun.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2skxcfbdy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2eiyzvsdd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rqvhssld.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nvakrrie.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsqklln.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ebfzvmne.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2inglxntk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2sdqqmjrq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2otbldhmd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jzwmolhk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mjpfgywg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2nxmcvayl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2crmcdqjz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mqamthwv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2symhaais.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ijvadbhe.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2mqhltriz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kgwnqzif.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2jjwiwykl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ontonfnm.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tlxniscf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lqcqfukf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nwpnklrg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2dhxohndb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fmsuqand.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kppnnqym.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xqdwudej.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2zyuwanxz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhkbwiv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2apzwasbm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2daekjtak.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2sybqslgo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ixcijzux.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zivpvril.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pjtpzgjk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dqowcscx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vuqttali.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nxmwzlcg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2hujdlsnv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2tasfiaoe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2sviuzyxy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qzczhmsn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2toojgwrv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ercowide.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2taxfcshx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2odvdmdax.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yygtoljp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2casnusqs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2yfrqlrpo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2mmmrdgga.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zyznssrm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gszitzti.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oivhneyk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gbkwbrrt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ywzacdeb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cdprwttq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxnmconi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2evwaozfr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwgoyqp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kdvzayww.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2smdnrned.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fytcnycd.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xzrprsxf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yfepwbpu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ecuxlnxp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wqpcmvcl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kmjxtiri.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhvvspsw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2febaxefo.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kjezcfvi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2bltgqwpp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qifaanbh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2bkfolikj.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2pixhzkry.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2alniggjl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2dgapzmro.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xlcfhoih.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xokqzlfb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcdkvamn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2hlrqvlef.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2suuvjfol.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2tfbtdmis.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2eofpuzuv.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wvblcrdc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2apvwgyaq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2zdzxlaib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqhuucfo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wbcwtdbx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ltwcuquh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2kuoblkxa.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lwhoprdm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mjxuwhrx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2sfkdsucl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2yorfnrtt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uhrnofsw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jtxvzvcz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vcmkqqgo.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qrvahpzd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2nedbswpm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ujpfnwjj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iukhlwis.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dkjnasrq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpjpyko.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ggbfxosc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhubqu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2iwnfzdqm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2frxsdzec.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dvoqoynd.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xcdkylqk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ppjgudlb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2uaojlidx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ofsgflth.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zecyajdt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2dqqbzloe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2prfzxyzr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ybukgxjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gfptrxby.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2edtbzktm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bethkhmv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jjuzqkmr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdbhdzu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mbpoizxk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dvusrbtc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ptzjxnok.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jnpabmxo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qgeficur.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2eokayhts.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2riqtwdks.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zuickhne.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vbvdlalo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rcshhomo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bkcibruv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2mlpjnylx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2cqchwtxx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2flsctgqo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2onkflhnn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2stfemoqu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pikznvjo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zikzphwz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iwgufmkp.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kzmysvmk.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dxvkspxg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kqzvadzp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dgeducuw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qiusysgf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2sofrdlcp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kbvvrgvk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vjantyxa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjrcxuec.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2dozoefbm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gdctunog.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2uqdbghxu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gywzweco.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2tflepdjo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vrpuqxzj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2faczsueo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2fbwnkdry.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fdaotsup.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2gnjfqefq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vmnwpnvw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2sodsffnx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2chlihtfc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bbpxfgxd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fznjxqni.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lrbotail.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ungemvzy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2grycsavc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kfdseivf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2khziylpb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dzvrosjx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2orvdclwu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2rdhrbglu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ubyioayz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jqyqprwt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vdielyew.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2gvbgnlxx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zypumizn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ycuityfm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jlkfpdvt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sdbxuezn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xpslnpph.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2kaskstst.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pluiaocb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ryvoqpem.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mjqrlzfq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mxbwiekx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2isriplec.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qyiwsygl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkzgdsrm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ppqdfywu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ayfgzziv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fcmsfgvu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fhcnpyif.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2clmaufkj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dnymqnfk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tejsdkul.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2uoqafywn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owsetduy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2gdejcovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrklgqei.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2nutgewnk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2usiximxf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2znnscujj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2eykzhycj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2aqlksyxf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jrmeszbd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2foddnlng.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zefyrzdr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hknthrxb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2updtcpmp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ulteuoju.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2vjvngvrk.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jhgipbee.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rmvvwihg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2daghdmfs.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2itpvhlbj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ochduxxz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2uwqduyfe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bsrgnvum.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2paktfrlr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yaeulzjl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tfbqtomn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gxlxvktt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rgziiesp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nfmgfovf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wggswcih.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2fbcpongk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kzepurxi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kfacoget.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jnqmvhfx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ppxbvkuy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2orbsaqyb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2loghdxcj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hmktorqf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qourwnvx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2yycxtwkr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yyoutmqc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2heubnpey.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2skwymxys.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2avftnvzq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uatiadij.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2doemnmce.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2okncktvm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2boftekhw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oogvfolg.html


<!-- 参考信息 -->