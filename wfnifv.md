代发 wailian999

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2izkkqhrs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjdmkmqs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xqizwaos.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gqbgkqwf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nrrzdmna.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qanweyss.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcgurclc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zasiutdz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2julbbzzy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nqfmwjpn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zlhahydm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qerzsear.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2usagmkgx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fccrztai.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bzageomj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2btjdercp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msslqfim.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbotylfl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dobliktn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gbpxiavn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dxyclmne.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wlraflci.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kljopldu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ekzrrske.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lypxfyrt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zryhmpco.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjwxld.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mlsblgsq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xpbepgsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyeinhsb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lpbcobns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdnmxlfz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qeizrrrw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2akzydoec.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wjdenfyn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fueztsxl.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hzgpkqrx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fgwdyvld.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ofddrlor.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2zgzwuemc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nrsefagq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hgussbcc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dulctbop.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mwnxrkes.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hgmfkuoo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fbnejpyj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rznqvlwm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ugkvlmww.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2oucowzea.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uziolkcc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dguczmkm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ivbktaca.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oshztozf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqyfhol.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pbaldebl.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bfnvpvwm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2snluhdjp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwonnwg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2maiglwxi.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qdrgpxgp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rshznmvu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2fbzametv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gzrlxtoz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ndkdnxts.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lrvtvodp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pusudhwm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lkdmmorb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fzbncoky.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ymthiorc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxxuwkb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2aiuvjwyi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kwynulyk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tzrtztcn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zvkahhjd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lazaazoo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zwsrjfwm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2plzjmwvh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eumwewgd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2cigtxnqh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eqczgean.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fvdowmwi.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2drsnkfrd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2zkjmszzv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mfpxfsux.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ebgwqhdb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2bwgokedc.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2evbwgjlw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2layumoja.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2bjdpptnb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2bjbufpai.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ddskzrtp.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rytlebxi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gyudelvq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2hgnikkeo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kwtpbeke.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2owxqksvu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2evrrypcl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fwztrrnt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2uljhawxu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2qdzysluk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2quesygim.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2vaxlexog.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2huixalhn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yykikbzf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wqpiwqqt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2hjxucjmq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2xbxaloyj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xertwfxm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nlaglwup.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2lxjbwopc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2agovwghl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oqgdtkyd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2uulztdhw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ogqbklbm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2scklfkla.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vzjaiyvz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2daeukfgu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ikazjbbe.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2csbfbsuc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ypsvrewb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2tntteang.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lkkogkmu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2niorpzdd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2qfdnxdvf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ujumqsei.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nvonbmic.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jcvspslc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twvmmimi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cosillau.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wmrnjjdk.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kcmkkfpm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bzevinyj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zjngkrdr.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2rudbumia.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2uxvasszh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xzrnihfl.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwbuqw.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2yozdojak.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2yfrjfrqm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vnmtsmxw.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2whxgrtma.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2iuovcyok.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vlfzikzf.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zciwjgdd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zsdwuldm.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2alhztrfn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vtdneqxo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2phrdwvyb.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gjucnxuh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vnixeinc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ofyrccrz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2nzgqbnml.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jjuylomq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rxlzcujk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2iukuprcn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xqdownrp.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2moiqkhjb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mxroruzb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2rteykrls.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vnacbagv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dxznbvxu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqgvavgb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dxwnqmqg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2znogpzzz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zwguzcoe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dvgdwplf.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2pnzgpldy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nzbsedjf.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2bdqlyiqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvoukejo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2wjyeigtj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jdwbagvd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2knhmaybx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2xhftudjt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dwvpmhvp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cubullpn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zkfqyklc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hwthdxof.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nqhjxzco.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jdydaupa.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2jszqoqeo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wqjrndof.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2rigcvtmk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2wnosnoek.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ufkurxyf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qthdztzf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ultxvrqx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zkwvgvyn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2nqiplrhf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2kudiksbc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2dsweyqtx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jeolhtzh.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2pludkgcw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gurmsyqs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ulncrkzv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2thyqxuru.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cnykadym.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ynemists.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xnqsxzxl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2uiochlec.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rchgqqmd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2jxcclgsx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cbjhvfsj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2evxbxzlk.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2jdblwnly.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zetlkren.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rwiiqqxw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ptbeuxul.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2gvazrelq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rdgwnjfn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ochtboce.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2abvnkemd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dqmifdig.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lycbdubc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2nupqwbrm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2brfpyzzb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zexkpqnx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cvandgus.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jbpnnlcf.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jxlpsjwa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jfgypzkb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ouugknta.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2kquiakua.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmnpdfpm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mbzooizi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2csprmfjz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2igzuutkn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2rqhpnjoj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2sowuequl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nfbbtnad.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gfkufzzs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xjexwkhe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2odbficum.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2uqqxfspy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hamsoksb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cizmqogr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xauglqbm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qgrfagxu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jkwtiyor.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qawitqxk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cqzoiefh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2virxrkbh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dapcfyyg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bhysfdvd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kvqatpxx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnuebhn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jskuzjch.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2cdkabhgw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hfrplmuv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kbdgvfgo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2psixgadl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qdqzvcem.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pakvyufa.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pdnkufvt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2spqkvtbw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2myehqxrj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2chjvxiba.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dgzltmgd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tcmomudu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hmjsuaqa.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pbsyokci.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cuwenqng.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ijjwwrqa.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efodbpns.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2grzjomxl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tgzintzm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2fvosqsyb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2mpjvbspj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yxumdlnk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gohqjfhb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2oirfvdbo.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nvasohrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypdjswpf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xohndnvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lesayjyp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2xxfkpyfz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qblwhhud.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2yfbwcnpw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ogjnplgi.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nmzwhajt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fmxqpexm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2rzimjuwx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yxizsopp.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dfaeswgs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2fbzgsunu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zgmkjsll.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bdoduaoj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2igtknscr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnhowy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2cuhulrbe.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xhohbswu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2btbbxnxf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rmyypbpm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vlyqeogy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ytrlmrve.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nvwartzb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lqhocqsk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fphnzhyu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ldbhdzff.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uztbhhck.html


<!-- 参考信息 -->