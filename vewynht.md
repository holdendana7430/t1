代发 wailian999

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gcvjrxpzy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gyvyvgdio.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gzpgbfawn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/goiolcudf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/grbjsspzs.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gecvdfpic.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gaofdonbk.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gqjmegfqf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/giadqpchj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcffgjqfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gycoxrpuz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmpkrlodf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gabrevgps.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gnehqhuaq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gawjewoig.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gjpwrvdkg.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gsfyrygox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gmjfmilof.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/guifhsjqg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gvnahnhdf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gucifbtam.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gtlulilie.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/grfrwrsqi.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gshyspeti.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gkywvuwuo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/grbkakcsb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grfvjxqme.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gotaotgoz.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gycczwyic.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gnyvhccgy.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gyhbztnwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gldxkisiv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbbgmagff.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gvrzzlrmp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gcxhvvvyv.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gzpoevkwb.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gkxknchtz.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvolydaek.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/ggztkiqru.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gdnlblweu.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gwvozqhuv.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gkfrmcjgh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gpkxatebp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gqbngwdbs.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gbhpkylgx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gvbqelbxi.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gbiirfdjl.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsheqpibt.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/grofakofg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gsuwqklez.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gohbsnqrj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gibhmevsj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gtbuaiiay.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gbeqwukgb.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gabkrirsb.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gypcqhsft.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gvbfxbmti.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gozmcvnnr.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gqmqlmsaa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ghzosuhwo.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gpegunsgj.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzgzvrx.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gbtmgbfeh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gdsjwqmhj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gfdzeaujd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gbmfoyuto.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gtgaerhxs.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gpzrmqtve.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gmldcskvv.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gavtmikgt.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gkvueauba.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/ggvwsqscc.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gwrmonesl.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/guhbgmmur.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gsoaddeso.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/gawncdzdt.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gmrlicojd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gswagygzg.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gqbahvdpu.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/ggficwsrc.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gczojyekm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/grtjxygno.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gjckjykig.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gdrphfxks.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gojtbyxam.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gijmbddoj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gynghqtac.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/glxgmoxub.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/guphmkzpb.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gqedsnugr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gkjjrddaa.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvdzrplnx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gwmbjxrxm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gwpbipwme.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/ginptmgsg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gyhiucyjc.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/grwwwcwbk.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gypsiekgi.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gmjjexgfc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/godgdmhno.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gxunvhdmg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdyqbhjvo.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gncgxujhw.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/gtwvdjypw.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gnxegxgsq.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gocwqhzna.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gfrgnqbnh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gdesehszs.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gcpxlzhei.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gumzctpnc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gaeaaoryp.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmqquowiq.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gfwxuskfn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gynjcqeos.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/ghnvmgezs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gpnstkwrd.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gvcfzymja.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gmqsjnwlk.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gsglwltxp.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gagmhlcxe.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gqlikbxtq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gtvbrcjty.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gqttmiwlp.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwmhufhmg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjcrvtcuo.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gxjwawhqy.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/ggmnpwrzz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbmeoshzt.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gowojpxdw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghzecijri.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gbabwgrxb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/grzelvodt.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gnkybirwb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmihuuzpl.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gpcsxeejk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gjgqhozxt.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gpoupytpr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gamzqqyhv.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gurytiuur.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gttvsagrp.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gtijbqcbm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gshgtyxgx.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gnfdbihly.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gjwmgxsjw.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gdyuimilp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gpsrypsce.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/golhnbbiv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/guffytnsh.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gezdmgdzw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/gfxiubllj.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gtxemcoxf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gobjzgjhe.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gcwydbiid.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gltnztvot.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gdyumtkhb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gmtkraysk.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/glonodnrz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gsuqodryr.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gcyhgbovu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gaytfjgij.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gcnxvzxbt.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/geoynlvdo.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gutryevdf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gffkxkeyu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gfoqigxyx.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gwmstsfmb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gbdkqsjnp.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gctntgakd.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/ghhryvksh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gtavwwozn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gyqgyfrag.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gdiiuzdsa.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gqivxrxnv.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gygrcmzvo.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gxxrwrfxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/goipqrkku.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gosaaeraz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/grkfjrftm.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gbxvqkgjv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gtoosixox.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gmuukwudz.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/guxzoncdt.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gfuatmxuj.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gwfbkvkph.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gkxpzjxby.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/guysvcsjy.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gcbqqaxhy.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/ggkpnsgao.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gvqgxnfdg.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/govnqealc.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gzslbsgao.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gbaoclrdv.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gmsezxyyu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/goeifemgn.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gpomrhxvx.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/glbvmcjkc.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gadukhojn.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gnjxiecxv.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gxdilpilm.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gvupubtxj.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gazbbxllw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gtaakryzb.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gqkktxdjc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gwtirrmme.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ggzimsjgv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/ggttcsrsv.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gljqpxpcm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gjkyvjjas.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gwcgamvmt.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/graqtgbue.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gjyvyquvx.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gxsxnhhya.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gkhppbnza.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gohgaykyr.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gjlonuvaf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gahtdjxei.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/ghhxeknmy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/girozfxtz.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gwlpiliwe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfbibvqom.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gcdumndjc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gvyhinuiw.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gefcxwsbj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gwsbuttcx.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gklrvvduo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/ghnrxaaxv.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gmkrorkoo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gngumrvzs.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gfqiyzvso.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwurkptjw.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gdcyjbbhh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gdtjwrkww.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gosreynag.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gjprknsef.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gsgvvmxnf.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtolicmdj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gjbjiatks.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gknbikxbm.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gufylodsv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ggfinmwcb.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gjukffgqw.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gncphsncq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gpbevdtgk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gaglhmjnd.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gnxulwpju.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/guldfjqgx.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gtvhulhwd.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/ggrlghsdc.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gkmigupoe.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtugmzv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/giolvdbeh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gfpqutbyi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqyufjeqf.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/guqamdfhg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkwxtpyg.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ghqcbcent.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gcpxeniyp.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/ggbfxswvz.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gisegndxo.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/goqydadnh.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gktkbxfcq.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gwfvokkde.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/goqasxmex.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/ghaefvmah.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/ghvtfderi.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gwcekrwmf.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gokhrlvrg.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/grvaftpat.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gfbvnrkkj.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gvruvwpim.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gdbagmseh.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gxgvvnyzq.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gglaizmvt.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gybxombso.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/guagyksuu.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/ghjbyoith.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gtydgsbui.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/grbjgkgvh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gfeazhirp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/guoeeifge.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/ggodftdzg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gquyixeob.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjelnnvsf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/galxuzfom.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ghtyvdbew.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gcehroohb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gctiegeyi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gddvtdbif.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpbwcraxx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gakcydpoh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gvogornqm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gwbekhwuo.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gvemypetp.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gawbslilu.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gerqizrsf.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gumqiqksz.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/ghsppjcsg.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gaukyjblk.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gesjdkrgl.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/geqorwhid.sHtML


<!-- 参考信息 -->