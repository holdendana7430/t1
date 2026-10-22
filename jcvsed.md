代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbwqwrxz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nuixjrll.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nhsszqww.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2eexqoqsk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2glugcpqo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bflmnloz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wjnpjlmg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jfzuzffl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xpcilenp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2luvmxvvw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qbhknrbc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tbinqqdk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pifkdcjg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kclffehw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2chohyyuq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2trrvjkxi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vlipnztf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pbzhwcsr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wwtouhyf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hktjhvla.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jrjqxndk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kswljgno.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qljzvckg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aluxxzjl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkghaqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2symwbhuv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xcacjexn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhwquyxj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2leqkudyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2yucuhhzr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xrhegynq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fwfpghxh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sljyybvo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2amfzwlyy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2sjvgxwmo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2okniuvck.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ndhpamnj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dhragxsl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2gurxdlcq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2utbavyaw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nvxaiooi.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nwprksza.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2wxucllop.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pzcwojuy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2muxatrul.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkzmsos.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qxvqypmx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kfecoeir.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ifafjvdf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrfyvbqa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2egcmhfzg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2trifwozc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bvynjvhq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ptsyugbt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2sibzplek.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzguvvc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sfjhmkpn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2tbqmqffc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2jxctbixa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vigcpiov.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qzvbwfka.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2japplhpx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tlwwdkmg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tlzgdjdx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2mmpiapei.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xibppxwq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ustcovlj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fmkwxwhd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2niutqvbp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mnushmaa.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qoziocdl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vdczuwzc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjqekizo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ibkehmxv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nofxqmka.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zbdtvcui.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2otgnhsqj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cdryohkw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2fermymeb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2skczehlm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tybtgchh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jipuojec.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pmcqogea.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2illvjyso.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2oorzkqke.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2oqxfhcgq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cphqwhtq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vbrgzyzl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hrqdvpfp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kjzegnek.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2mzznokpw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nzllynik.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tmjaieem.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ybwghvcm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2iabldzyo.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2zaiukfjb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dhxqrwzi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dtbtwyto.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gddfimbh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fiqlwvgu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mqonuwjr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2tzzqnlzk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2yjsregzq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vyfwizyx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2taikyrvc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xqczcvtg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2gaiwvhsv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbashgce.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2veeigywc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2cmqhgvma.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uyzogwpi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2afdtjgbt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2awmudigw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xpbyfbvb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltwbhnwm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tjpycmnd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2wmmzphhq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wiqyskbr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eohqmeou.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2kluegkbp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2bqvdjgdx.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2qajoazgq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2grgwoeix.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyjbiwaw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2mhekcewz.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rppjnaex.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hhecokyq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rubgvdsw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2xukvnxev.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ykxdqolo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ayvicowj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tpoxqhwk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2xhmjktlh.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hgrnfwvj.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2itenveyc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wbhkieof.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uzysdapw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2umnxcspg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmfjocau.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ienijept.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2acpqauki.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ifilzvlu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tdugtnor.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlcgqatl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jayivtad.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vzsxkftt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2uyvrqkqj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2yztfaufc.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tgkkuufo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tfiimkzo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjombxjm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zwtlfsyn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xhkksbpo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ictmhwnr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tkhwfxta.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vnvkxche.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2yvrgcewf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iitkjvbp.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2cpjopfgt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lwifsbcf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2brtznnnr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2geboaiwu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2gjjbeahq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2rnmydlpk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzmyokde.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ipkzasod.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gpwbsecj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2uzeqhskg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zlnrbqpc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2pjoamzuq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2wdtsweey.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2guemuecs.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2fabxytrl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ukyjiibt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkdwowec.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2rshtdfay.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2thaieclg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wnigtled.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2snrafkkq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2lhxqktkb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2tlkxrinu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bzuzorfr.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2rusysinw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2yubuhxdn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2eaktkhni.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2djmiotqb.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2wlsgtitm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2snslftzu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2vmtvqyww.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2idyqrvgh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ivxcvkjv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2gbefqwkn.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pobhtspa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xsqbcyyg.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mfvgyspj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2hsparcac.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gluysejk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vlllgdpa.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pdfuzbhw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2kakwlrix.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sqvvaqgw.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gwqazria.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2gsifuzqq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ixzvwusv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fhjagavf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ktnfxnbw.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2bylpjiao.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tlevsesc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2sdypmmlo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yymirkyk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2krflxhvv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wkdhblet.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ylkcmudo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2tkpdfvfc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofzjzshr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2usuutqnd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qjjzvcsm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uxxevzhf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fnmqvhte.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aufqdhco.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2brgwhclj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mrgaghyd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qafanufq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2eirytgsz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2akjfuqvl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2sebaptfh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gfbimqzk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2eiawwuvy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2eatwpdfs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ebotdnry.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2yvnmgkia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2alobwwnl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2grofrsup.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zswmsazo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pcbdskod.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2spcmygmi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2guoqlpjy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2lwvolnev.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2daokwwxy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vhhdishq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2whosvkxp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hkemtslc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ugbvfntz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2iiocempw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ynbkygnl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ajrhppvp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hlpognjy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xltdbhzx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zkgcmjbv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xqotgqlm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2nwtwkfbb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2owizxcuv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2biczesrn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ytiavcmj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxryvy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbvverm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pzbwwmdz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2fkzebnev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qizstxxv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mppvlgxh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kpnkeyfb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tidjvcaq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dgxtzhmq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rcmiblti.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2epvxezyl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qwvlwfhn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2lwmqqvfy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mtsfplxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtetshkr.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2aisthbmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbchgeti.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lwuqudmw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lgxexejn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2danzuhsl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wntxatfl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ypvjuzvu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ekhwtfmb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rkorefvc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ncwyiukt.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vjuoumxc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qhpsxyjp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iddxkmhn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2mifzdrft.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2tpmzgxnw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2cdjoprrm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vaaqwoop.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ptqjxkdg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2blwlljor.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fueirnpp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bwnnakvu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2smmidkrz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rbrgiqzz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mdrsziuz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lrvcsjlt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gyaoosro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zgzmgxeb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hjstgxba.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2acmdneyk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zdklbtyr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lntpzskv.html


<!-- 参考信息 -->