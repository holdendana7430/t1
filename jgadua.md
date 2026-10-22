代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2reczwgbb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sknwjbau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2chgepwnw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2olfvmsmk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jflpswgp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dnmvvuzr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pqcfbrcx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ahdwnreh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ngbszlvw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2scctotkq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qroxkzwj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rxoajluj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hbzlxvuj.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tbkxlrxy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bpxvvocq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jbyfedln.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zgwtqbkh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dzeauqsa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdbifui.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2euasdnjc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2loyttliz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbablxac.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zqpcnlho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drjwbuzw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2cefdvvtm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2pyvukfwt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cxbujkzo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qrsbxizx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hlobvuxv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qlwewiuq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2synlzuus.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yfexmkuy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2aqsuvmmh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tszewesx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2lqvefcvm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ynmpfumw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2xedembae.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2dsikytmd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2iorseuvl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hrxaqvcf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hcfimxyl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qfjylier.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2iqjezenu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ohlqfdbb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2mojgmoaf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2klbbyrzt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzhivvsu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwyuqhsu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2somrjgzl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2onfylubw.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2wrtaxncq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgoshxja.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wyutrwqk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2robjdqva.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2lcikymhi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2dbbunosh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bdzdodbh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2aikukqsw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ponrlbeq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dbjmfiwe.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xlkdiyas.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cykmppku.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wxgvmqch.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2izcqmawg.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ohkfumrp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2jghaupqk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vuabvizh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bmfiblyu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kzhyaxsy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2odlzdery.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iayhpndn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2whgswyrr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oxjkqnza.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpsqqva.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hpzxniac.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2htiivsme.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2anecaiwx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2hddoqcbj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2atayhext.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zidubrvc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jubjdcnw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2jlvwkxbd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wjzsrxye.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2prlfklyp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fgxjmiue.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mwlmqdol.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xefloscr.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ydyipohy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2yzjarahf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2jlhpooae.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2affslppd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cnknxhhx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ksdhomgk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyuroti.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ydolyord.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ayzuditq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xhauxjvv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hzbsewcx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2lsblqjhw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2njsnfzza.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rqhbvbxl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvisja.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aiisxpqs.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgspgyko.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2bdthrkcv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qibdjghw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2snwtvwrh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2targecwd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gjvgrgto.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2eqfhwzgn.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkarmqwv.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ylnyousi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ttempfef.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ubsuzptx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bjceagab.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kcemdluu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2vedungrv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ccjoavrw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hkiiqneb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rojtqlaw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jxecaowb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2goyiurbf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qkvuummx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2aqfmkuli.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ydmkwpqm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2evyvpxbx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2evswuguy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nbbxgjxt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hkdzdaqq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2icakkogp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2pivfkrhe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jvbnhgxr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fqjheruv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iauzswxo.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyddicui.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2shnduiix.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ubgsfxyq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2sqoezbkw.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2hgxibsgy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2foedtrrf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2xunykmkl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqpztl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qcrzutxv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xsbddhwm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2qxdfjsog.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdcmavlq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2yswgolvd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2egsqdyvy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fijoqoht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fwpeglbs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2dmqnupty.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gidteaec.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wqjojijj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kimjhadx.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2igarihah.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yodrcaya.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2trxthwqb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2ectsjuly.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2bbglrmrw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2apyjvbar.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mddshbck.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2umxtyazu.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ahjqoaav.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2eudrivxn.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wqnggybd.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fmgdnxlq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2usngqtbo.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2fqfjjvvm.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2tbqczyxx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrdspcm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ecgjhnhx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2kglhesne.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2nwtjpdtd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2fcznsrff.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2xfiqsbpk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2aswndehj.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2eaewtffc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ifmdnaor.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vqnmqfgq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mmwkamro.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hsffrmsf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2fomdcgee.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vkrpqwkz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cagghddz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wjqhilgd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2vzncrpsn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2hvnlhslz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xwuszknr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2uesavvkm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ofnmnngq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xyagiwkn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fsooakkw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vmmpgqjg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2syktkitd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ssjnoslz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ycaljoyd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2twexkauj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zxvnsapw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ezeqxlwb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ljttwetr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ddqczkpw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tkzhozye.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hyjvrdxu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqqgngzd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nfyiykcd.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2axqkysjz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nhmxuaxi.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2noqtyyet.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lpdxuhmx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uzmlfbjs.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2haqkstbf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2srfkfjpe.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2kiljpjec.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pbhyotxh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2njcvfmww.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgenxcwx.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dvkhqmfe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jhbkdgvk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iiejhdri.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fgycrjnq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wcsrdlgl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fdniunwi.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ncovqvmq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zahgapio.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2blvzfvox.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2mowvdtdq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yuuexfkl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2dsxdplmj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tungeelk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2gaolnaxc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jtnuehkj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxybytyu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2qmwbsoph.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uamgppac.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2exwqykxz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2usgpzhws.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2axgsgart.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ftsdyhrd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2eqrdqyff.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ccmokvfe.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2grnsyuxr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bmzjowgi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2muvwjodk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tovkuisr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zlwraxnm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2unbrthxc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2axaiclql.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkrhuzml.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tdlswpqh.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hjxfwmxw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yclrghaf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zacjpqph.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nwwbxjng.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2kzfqrnor.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nrnacaut.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dfbhbipm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rvkqkhjc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hwuiqmfp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2giqlhskv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ddbhrdbs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dovxsmdw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2uinteunj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tmolabkj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2oawtafdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opydplxz.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jbajinvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzxoitnm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2jbdsgxlm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2aorovkvi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ixuyqzli.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jdicdiln.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tjfdkgqx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wxrfseyc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dgfgsfpe.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ewecefjx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2boxksfzf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rxfukzcx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2puzckhgd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rukwycna.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2yjugmdyx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ibmfmprt.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2omxyqfab.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uqcieqxb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2wknodjid.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2btellcby.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yjhmgbrw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ddgxirbb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ojanrqfs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cxhkpggi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gxbqcawq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sxunywua.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lapkiubt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ifccdgcw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2beygnnvq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ourmdhcu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gznbmeua.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2stftkwge.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yhrjwfto.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dubsjigt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2oyidhltk.html


<!-- 参考信息 -->