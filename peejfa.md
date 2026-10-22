代发 wailian999

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2estsojsy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uknmobhg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnktcgag.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2aknmadld.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaifnnzs.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iruvijcw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2klpxcecz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2iworoboq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tgikdlde.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oheaqfem.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2iciurrlk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vqabcupd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zdxyfwok.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ntqcyhmi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yflcddqf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wdeyzvnl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2geoccbyg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hvhjeclk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gtgpbrtn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wzjocmdb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sevvieyl.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2pbfjczzt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qnncbsrk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2whmhwnhv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xqcvcfos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xumuzqkl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xnmriwdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcnvfiks.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ppokgvbs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lnyrmevk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2mjiwpwtr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nummovon.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yeqsnlkg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2jkiwxxap.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ypvyqjvu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2znfrqrrc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2npkefcxm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qfatyari.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2kzazspid.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wewmjbxb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vlxutyxz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mtvmppwn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2abqpomqy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zcqqakck.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2oiegckni.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fttqkfgf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bsfrzbsu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2sfbobnpl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mpdxqjil.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2oelegeak.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2riyzqwqg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zxzlvfae.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2nvkebzvn.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnznbv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ojrpivkx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uewennbb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vvhlkikk.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2svzgkqar.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zfbkqifp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uidwfdfd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qhduepin.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dangsdia.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gishbgxx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2oiotzocx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ebnlkuny.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gillxfxn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qdkmjvzl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lzgvsmnj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zdqhoipb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ppzqtkka.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2whlwlgbe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2lqgskywz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ttpqyeka.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2axcbrqpo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ismytikh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyigsm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uvmjqkrf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pplsckzn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rvyixzdy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2dnoosduy.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zaelyigo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2oitiksny.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jvtvwqpt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2idhgwzbh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vkziillc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2irdxtpgb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hlcwhgcc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2lpqhjybn.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lgixfyte.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ynolvfkp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2vkelcgzn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2qpufmndj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2usyugnst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2alxyblzg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2usljscwl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwhxinp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xmtererm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2wormdiza.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xkppulhr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfbqazq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2yjqafaif.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2kgyaroso.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2iidnmbsf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cadpqvzz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tubddcrf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2zgnrtugb.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2bwlrggxf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bzvpxklx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dlxquauo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2pbbkuewa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dxcauxpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtoqywna.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xnqtbbhq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mmrttanh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2hidbtfmn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vpplwoei.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxhbgalv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2onrhwuut.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2cnjoawiw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2glpqanei.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2rkjozwtk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2etmjgiee.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mdlhfejn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2bvaxwfdc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2rleoyhjy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2snihbdov.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2tzfgqjfk.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2pqcrmryp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2mnwhtfeo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2kroadvvh.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2lmursiua.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2jlpatijo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gqmzpbzq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2zxzhrfti.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2zpbngvuy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yopvgnoz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cdqimhqj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2oshnohck.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mcukyeku.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bbwufkcz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hvpwxpsr.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2clogkboo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2shpdkpko.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2rlxodpdw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ocqslqdw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cdpthzrz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2txwrbraw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2caucittk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nonhsehw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfqrftz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ocmmzxxp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yepprysz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2olcfblqu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2tutvqdfw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2igbrjive.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2nkkselon.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2pjmjfzbf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udoydbgu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tcfxzqpo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dqlpbosc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2nmurkmma.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2oisxsvww.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hzkuujab.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qoqbeswr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2veujkuwx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cnktxicp.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rikjjkdf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yxpxhmew.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fajonogk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2trubncln.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2nebkuhly.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2zzhtmnzh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hnotgzxz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2xmruibsc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2apkqhmuc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2cwhkzfvv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2dmmwnufp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2idsyuknd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2mcbjmtus.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2czuggtsu.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aytwnyhv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2odaremfa.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hedhkzap.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2yxsgrdcj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2nuuqnjdv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tqcumpvy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ajuubxoz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kyvicxos.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jtljjpvh.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2aersnizs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vxvfolax.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2dyekwkof.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kipuuxed.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2elxhiaxx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2zygnsqel.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cdtrsgef.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2ldxzlynz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2djxxbdxq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2opcqryts.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cbhjleca.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zrxevtag.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yeufwxqx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ibsybqbj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ojihhdoh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2wkcmkzud.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lfuxagof.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2brouaors.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yiaveqmf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2csudbhdj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rihtnjrq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kfkddffn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2znuxkigq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfhidhsx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2vkqgewqm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfeokskv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ilvepnyg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ydkgdvrm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cvtxmzsn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tskvfuvj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdhuazj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dsrlvink.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gntenyvz.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zcnenivz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ebpzobbb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ickwiowp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dnywsdjs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ekwzlnpj.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2izzuvxfy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mzlqmcov.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2sbkgbwrr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hfvdgyvx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2waqxgoxt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2lwhpbvft.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rlswvjkx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hccxaexs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ooqzfabe.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2dbrtyrdo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bwqfmubz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yfssubkm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2szbchjhw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2awbsdipb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nfadaqgn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kkddpxve.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2megmzruw.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sexgqjlm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qtqawytk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dgalnydi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2unyamfsu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xezwtltf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nnujnyqy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2njuijubm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cnptmisx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qkpwacxc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mlxglbrf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qplfkcmv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ntokaany.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zsdshyge.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nagbstri.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qabsdyjc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtthroqb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gxishpoa.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dnktbvhe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2yqskycfp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2sjkdycas.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dqwkmqwd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2iekqdecb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2gynusfuk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bvivgpxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihymvnpw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2dfdtndim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kajfdogt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uavinmma.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hlrcwcmn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2znhyhndh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kfchdxnn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2oyockdij.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ldhzpmrf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uhifwwct.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jfcvgqno.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tbfbgmsh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ktxukqls.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2alpcnjdg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2arrkyikb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2awxukaft.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cczaydyh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hdmvwufl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2pvbhzzgs.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hinymvxi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hazlvicn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eyxdmnxk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2dwqpkywf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2edvmtcwt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qlukduhu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tgbxgukh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nzonrpuo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2izjsobxt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dlsptucv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wiolnhdq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cewarhwm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zyhamrjk.html


<!-- 参考信息 -->