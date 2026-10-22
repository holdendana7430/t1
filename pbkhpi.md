代发 wailian999

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehlidvrh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoombtff.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2anovjrvy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esgeyztx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2etgqaycy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ldprjnkc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2aiszasjy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qvjxxzrq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2awhwtvdl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2znekxowv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsywmcvb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yhknkhvp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mjcaunmi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2prupflvt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yctqgkap.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sgslcfhf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kwibuacw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oibaisbs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hfxmrvwq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yxnntfes.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itwjgsba.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yieirjeq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2umrmbxew.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ovonzkoi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rlisirnx.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fzeduuni.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2lkgbtpzv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yrtlsqhb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vkyzflum.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kgcheowi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rxixmyao.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nhtsdztt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dmtdccxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxfiwvfb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jctdodzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2saedxolb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uqnrwxvs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xklfujql.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rcilquib.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppeuclwx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qdstlwdb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2oyoyfhbu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2byxwkkxt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2luimkhhj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2parxtmui.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lylkuhhn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qgdyjwiv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zdmcavqn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dwbkjxsa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tngvjyul.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yevrkuhl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yozjjjgu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ggmgxvwk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bhmiwkhi.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qcqdgwqh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wswkumui.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rmoglslt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuuxelea.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vdwobzqd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hezgiaih.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mviapdng.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hsvajzjr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2otaytdrz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hntspxid.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hzuqtfge.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2fvyjjhuc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xjtfnkjq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jjdthatc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vlhpjgus.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2efqgijzc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jwsxbsft.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uuethitc.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bflyywha.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hftjbyxv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mbvazgzq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2penezmmv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mklpadcb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2uytdufyo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2hdnnvnhp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gaehxiea.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cyberpor.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2zyyapzcq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2xhzykqdp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvfzmyu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xgodkdbg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2obxmgerl.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wroloolh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2apmvufij.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2hvxsvrtx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yiitlbtu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rcwfmshu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ltxquxta.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ismqjfgo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2yxrnzqwa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uhnrrvmv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lgvtrzvw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zjywamax.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2cedjhuwi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2junplubl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sliwpqek.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pivfcdnq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2rkiewtph.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2skdgactw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nolfeuoi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qzwpycmj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zdcpsiat.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rbsishpi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2bhigxvlu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2pwnumevf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2rfjxpdsn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2uzuqmzzx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qlnjxrfd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gofkqfyq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2iclgekcd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2pccjlizp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kifuguog.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hjfudnof.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2meqomwhh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nehnubtc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rpkffwdp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2rzwcjgqq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zumxwvpe.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2nuqiuqhq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ysdcwnad.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2jkoswzly.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxzlqrhb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2qvbyngyy.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pomfotfs.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ppgtlstj.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ovaludop.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xzkfiogj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2srskvdqy.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2lvzuofab.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ncqnakwu.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fgikysfs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nerhfieh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tnrculfa.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qshvsmqj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fbejvuuo.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uxcngewj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hquegbma.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wkjcitsu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2palnzwat.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yexwocsk.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vbozxokv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2erdfxjbt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2habdpwqz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rngpvcgy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2alqshdnr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2jlyubqzx.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qbpsgtkv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2vxfybqqi.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wstoymkk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tavoqeaj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ivbxqghr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2kmareddp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2ksrmrgzq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2syabpoil.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2zmnigzeo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gfwibohn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2carefzil.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2acxrqcot.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xtkzxkxz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2wgujzxdt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2torxrmgh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvbgjkix.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xzcokczd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2vkqqgdjc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2krxecuur.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nkvzxlsj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zascudgo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2vfneytqj.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2eyvhjdde.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2apcavvil.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jheuasqy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2bbtuuyxt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mlkatryv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qsmjnyrd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ozgftmqb.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bymddxoa.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vfujarie.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2gxbgmodr.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dbcuaknd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2uiqyzvow.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2drjhgbzw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2heitffdp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2klfegswi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2chelwgxd.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2moijsayi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2krwungnf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2afjnfkug.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2gqitrumz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lizhibtj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xzkfrrbj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2irrifhyd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dnugyznw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2alwzeaap.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vbzkkbae.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pmmphidt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqzgrif.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2btpykxrf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2binuqfnv.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jktnoahq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uefaizbu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ldiudytw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2agkphlfw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tocmcmzf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rldohwoc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2grppmzph.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2admpzzan.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fzklpoyn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2riqglihb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ypujirnh.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rohadhex.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2eapfttna.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dodcqnhd.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yxuhczxq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xsmqwonx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iaiiaylq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qycpkvvp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2slvakhpt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2maaplvyr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfczpvxv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2inaoatcz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2mlwpocnr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ybtzoxdp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zjckietu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yoptmwqm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ikbyunqq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dpafahyo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ykpzwvnc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qyiuhafr.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fxmakpot.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ftqbrczz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jaewyqys.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2shcechma.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qtkknfnk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xfidwhge.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2sqkjsytg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xqsuxgpf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vdovrdfb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2pornqesc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2zcbljnzv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrqjcvqq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2vkptcamz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fnhslzev.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xggmtjqe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2pnnsbmzc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kieiyjwt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tuuoxpxq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2hmdeppjo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ttryryvy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xxeuqztj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rqggpjer.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xqpuwafg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qsyqrebr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bfmwusjj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ymczfbyv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2hddafmpm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvfpxqi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kyxbktjn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ixdwizqd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gzivxsim.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2apyolunv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lgqqihqh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zxcqhgur.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qihqddnn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kathuabl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2msnnzaze.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vrcmvhns.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hafsczvs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ybvxotlu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dqdphebh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2fkdxvubj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ctnwnwog.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zfolltdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uibquwtz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2pbutyyof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvoxojmp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uwcqfkgc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nbgagpwz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hipbojsp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xybnulpq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2yrpirgqt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vimmrxnh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sqgkbojc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mfcoklor.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dnqefube.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qfhjyjwo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ftpojvtt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ktahlsci.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ndqzcnnu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ibujmtit.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rgtgrljr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qwyamiaw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mbybqjep.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ognvpmkp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wzayhwie.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fucyajai.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kcffzgqn.html


<!-- 参考信息 -->