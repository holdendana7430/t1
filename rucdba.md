代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2metezqxg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zmpluyyz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxpefqle.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qsntjywi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfyxmdv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iluowacr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ujpcnfyt.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bszusgng.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tooaqkme.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jrbqtytd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pcdrfeii.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ildohawk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azarcwuw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bajsvmgg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2toawxkbs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2vumyemai.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2synubxdi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2idjwhyox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2abgdgetx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tocvyxlm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mfsayfiv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ivdsotqn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vafriafz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2omdooggt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wrzhaosl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdxwvbfo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qhacyqzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2behsvues.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nercdpqs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ydetnjsg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gctlxmzf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmrbdshb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cjlxtfhi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2tcazznad.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2squvcwyk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2iaibgdwh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nsvqeokx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wspkhboe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2zimeqbib.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rmappwit.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zdyexnul.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zjznvvwu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wdviugpa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wcbleufa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gwxnhioy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rgckygdc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqqmjwab.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gqixgsoa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cpcfmerw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cuztqqoy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xnywlfcv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fmpbwzpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bqjhuecm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zxspdhwc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2nopzjlgr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2olobhyfc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zgdjmjhi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fimwchoq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dhkjmtmh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fibsdndv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ybhxieid.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2balgrfwn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xrveztbf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2slpdgkle.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2khyxoumk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ppkccdez.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jrslaeap.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2twwxvnqo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2omcowkkc.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2piuechgc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ifwktupl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2btasktlh.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqkzatue.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ynubukon.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2rcoqcmyr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ijfhfwdg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2bapxrfeo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wnycxdgw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bvxyqaxz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gzxrlkzd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2lbxexxso.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xfdkrjzf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2cqycytyn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ofudghim.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fbnhtybt.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uyyapiih.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2faxelgpy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ddnbohes.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lbczypfx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gzksocsz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hlkiiowx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vkjegodg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hmfmlgsp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ajjylxhw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2odngpakn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvrqutc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hccvkwab.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqkyffb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2iwademgb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyorxdj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hytqiofa.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2eshatsck.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ymoepkxj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2bwtcdhea.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hemgnpcp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xddtrplx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2pjtinmnv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekvxkjdo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2npfymbbc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2iucrridt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2qiuaccrx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tcybqlqo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jhrtdmte.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2jcyuphhp.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsyqkzyb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uloexcqh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ehykmgci.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrgustro.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2glsrijyv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2smrxxxir.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltltmmvh.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2pslnrvph.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ygnobbzv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mkbryhjx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2awtlvnqk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2qqqubycc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2zuovgjdp.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mmjpkcvq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zjznbzvm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2gioyvzfs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2puhqnycz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2oqstgyyu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zcgzaedh.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ukkqfgbz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rrctdwuw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2pfoddszh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aqezsumk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2owsneier.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2tdmgtvmk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibtqddic.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bjwrazjq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2vtbfqrmn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2xtgsuike.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2eaumpptu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2hggscaja.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2aqcdkfuu.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ulqssmux.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2tuzshfcn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2nmhrjcsd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rerubtzp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2nxgodxre.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vucyesoe.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2isclvjzw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2yohgiatj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzmxhptc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2acwwiswy.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sajpewfj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pwpbojaj.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rqcmnlka.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jwoziczg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2fuvmdxvd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qrvajnxx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ikkpklfo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cpagsnih.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qakuluih.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zclwmxpx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2dqqwfigy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dhptdyrx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2itjefbft.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gpgxjadv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2udzckall.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2orclrcem.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oycrbwfc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hutemvon.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kmtpzxud.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pcqgevqb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2igmjkzyd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2uyoinzwv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2dwxhpywk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2nroztaoy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2tzytkbbj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oisxkxww.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2suaeeorw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2lsqtnbil.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2fwryrvqh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qgovwewk.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2vhnjlkxw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2lmgvfzci.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2oipvsddc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2joaskdqi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2cdufydoj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fqapyejs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zskurgtv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdrywjrq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2chtzrjjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2foxjzsbz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2nuqpajku.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hgurnjfb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2awfnxtrq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mvhhsbas.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pjufmcxm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtavsc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2eibmulck.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2zvwyiaub.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2agkdojgq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dwqhbdny.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zzczpicq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wmftceoi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jazxhkvj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2muzdbzxr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gxmxeekg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swpkcuob.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nkxivlaw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gvimftbo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2utwnyjjr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rzpdkmnd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2peictltq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2konwjctm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wcebrocx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgzftni.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2arzbjpks.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2knitlnzy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ozqlyvgn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbywqozq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2zlwtriqr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rhbzvnwe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kplbzrqs.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qadnqqdl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2oaletrws.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2zfyvavsq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2otmyumpz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2xbscbslz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vgplfuxu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tzzsfpsd.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jylmgwmh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dclmyjfd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2sycamvek.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mncinaxl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vnbxvqdu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2aebafjjj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uloifusu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ibvkwvpk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kifgidej.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vluxuhwt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jcchsqis.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2furmaykj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2qaiwniga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2rbnzwauo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wjorzkpp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2lptugrop.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tkovgpmp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zaqucndh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ndpflqak.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wishqmhw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ovbotwuc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtefjii.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gutnlfbm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nktytrqw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ccrdyahi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xdascevm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xbilsiii.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aixubpzi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qffnvtgd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dyznbyxm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ihscofwz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mblnzpga.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fyewomvn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2agjefstc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odukghab.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qrchbnsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzxcyidh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2knkeuhsv.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pfcemxgr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cgqdeybf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2moypnwpu.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ixhtuoci.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rnbtwpte.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dlxajmzk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sckbnbju.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bppemqsz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2mohlgtmh.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ykpokcwg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pfpuihnd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2woasfssu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2adgjbhma.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vstvaoyn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2femshwbd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2htmgdzau.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dapofevh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pqjbokgb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2aknkdygg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2sdzdmjeq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zpwfpziq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vicuwlsb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2luzdnmjc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bigjuwks.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2bgspzdaq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2luvzhoyt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ttnwikis.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yihrzmbj.html


<!-- 参考信息 -->