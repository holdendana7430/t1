代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3thxdpler.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gairekau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gkknkqbz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dlbccggq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rrlvqozg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bnajwupe.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tipxljzz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lfdapude.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkqjwrpe.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rzjbpwhq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lnvwrqxs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3zqvdeogv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vjvggpcy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nfezaanx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zlebewgp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3eocwhlbm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kiolbijq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zkyxcooz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zrxaesqz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pejtuohm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fcbrunua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtgiiffs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jeewlfvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3filjnsag.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wspyifkp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3tllxkins.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rznwvkeu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ytkmzsph.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yjmdagsl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wijzdlje.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ierhsyvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3gehqrhho.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hfyikghp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jjggbmqn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fdxqzwoa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3hdznpobd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3milrdnom.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3olarqjty.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dsqpcnco.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ppxdavmm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lgzgswxx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3behdvpnr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3tbsaafyx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3huvtjlep.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ddybqaqd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gtfnlrhf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3djuksnju.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzryngw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3itcqnvfn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ppiauchk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fergxfms.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ltsafvhl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pbzwvifg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cicfvazj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3shcchvvx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nudcdpqy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cdvqrmrs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3brvdakav.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uyvdtzoc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qqocihma.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jrhhtsib.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmdkvks.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3otnmfcse.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xglgmyth.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ngfvltwu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fdkfekna.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3znhsihni.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3abkinaeg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vevjrwrj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3leqwqybv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmgingrf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aitxwalh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bwdixvab.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nkvmqret.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3gxnhhhdw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3thfgvkmo.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3owcavlvm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hvdssdsx.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rtprljhm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3btuguzan.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3pmyiosfw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ufpwiaun.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3udyzvwre.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3duzjkpwg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wmtkmopm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gaojvrzv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rbxwuogl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3gtzsuaxq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wwtrevug.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ybiyckcb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3eravurqd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dkyitdtw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wuzsgedg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xwdoxydy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3thakjsdq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jtnnejjp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ovmfrjmj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gpyuhtxg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3awwjlrkt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nomhqlyo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xxmclskj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3vkashotz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3tkyprytp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ytbrrfle.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3pbsitami.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3anxcxckv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3jttatggr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kkhlncls.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wcvharty.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zvrvenih.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3jteykrxq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3arnekowj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3cuhtrvde.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlybpywu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xxyqizzf.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qhwpoqha.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vfixxgui.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3czuuhsgn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eqwsotjk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvqlbslj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pvcunflm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3uhnpidhl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ghqfijfx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gyakwkcc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3tmhkxpya.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xpnrlgpf.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mnfulygg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hyrwrdfe.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gcxetfus.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3srxngqdc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dgvftwhu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ioxmxeto.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pwbyfjzp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hfgqzque.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qynyfaqb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grhtehti.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3muiyirsl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqqoocyg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ztjdjwuj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3lnpktbyg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uvirgfyc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ntpuaiol.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cigezcct.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lvccwozm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ylmsaapt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezbswlvg.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bmacjvfe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cvlcstoo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lqjcbsxd.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ndjxhdwa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jpndopiw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3godkvgee.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3icjkrhuy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zplmflwq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3bmqkkhns.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3bxpyveuf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3bxapyslq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3oxruuaai.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yzvkzypc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3mkzmeeyo.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zosotynf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3qdrzatrt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3mnzffpkh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3jxyuexqu.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jgldfgug.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3clannljk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xztwiofc.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3apygshkh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ryvrtkid.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3mzheqkns.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ubodqnql.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hfmzsion.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3fquuwaat.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3jqtpgkml.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3tuejxhvx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3hummzikf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3awhdpqsy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bpjrukzu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3uqfqbhop.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3djllgmaf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3meszvowg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hcihsxlx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cwlyuxjw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ofbenwuw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jppbrsec.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3lkkpjnmq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mpjzlwcc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3aeivllkl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nqspytsz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ylhhgyyj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tcoytzxi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mvkxakwq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3rstwosiq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zlloeacb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wqiqjiml.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vxwctldt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3dhyufvsq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkcfci.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3isjqabpy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3fzosxdpc.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ljsaolrc.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yytaobxh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3btxynibu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gbmwisar.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3byqjctew.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wrsdxkvp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uaqjsvsr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qnuytrxj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fspfbsgq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nujvwucr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdgoybxg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fxumwhep.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jwnzeiyc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3qdbmxyed.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ajiuunsk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sqnpsbot.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yekryevv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uznvrlln.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ruxudcgv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssbzaqis.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qmguouxi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mfayvndy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wkhqqjul.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3yvulfaju.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yxxhvwdv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lhkkptyh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mkhcrpts.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tzxsygih.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3hcrooazp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qxgenigv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uffflxbe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fclilbqc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xqhqaziq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dcstysrd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lhvyuuvx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3evkzweke.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oyyvxfei.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkyluxl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nclexqrz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3txfafqxr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ulbrvqlt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kjtgeqna.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ynahlavo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvhpgi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ulygnmae.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mzlimxmb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wjfvbybe.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ceniygbf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3niawewrv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vgxuqokg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lihfltwq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hzetrqkt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jfjlberk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vbaxicxb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3aynkmbjm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brlcatyr.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dcarvkah.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ohdgtgrb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mlvkhozm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xobfzubk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3qutumzvg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3obillvfe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3tdfnksdm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xiibknhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzilvznm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lcqafbtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqjenrgc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xgenpalq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ffaqntht.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jgclhiqv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pseqyodo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3dnyjgwln.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3crgudmql.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3alrsibyb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ikwozsfx.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3melnkung.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3luhvyjbs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3gpxptdex.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tcnvtusy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dabsrqor.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ivedyrnl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jwnfthjk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3upnfyfed.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jcpsuaoz.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mzgpthal.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dnpjmkzn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3nfwaipsz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dvcepcqa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3abepcbsh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qxuxoica.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ojujqfrb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3dssyeynt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3kdekckxu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ugoyqfuw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jfnfrqgg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3aduulzld.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zkzuyuqu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zokflpav.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vzfmdyxs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3flzkvjpi.html


<!-- 参考信息 -->