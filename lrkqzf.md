代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3syukvzua.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofxrnofy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yevzbdwp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tfqthecr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xtwwngkr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llpzqlky.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oelmdpza.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ydkydyej.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3taxeziqr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nlxdaqum.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxbnoq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nzndvgqu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3znzcwvbj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qnjysbzb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nygmyadm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ujuyyrgs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3artthycv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vdxgbuif.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyyhihuo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fjcawznm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yknwwnnq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fjmxtjcy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvnhuefr.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yxpryzjb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3obezwdim.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3nkxavkfl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lclwsaqk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rmumroxo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3xwjawqgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ridzystk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tshhsejy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fosfvxkx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3uloqbfmg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3seeajopl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xuvytgbo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hcntybek.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3pvorkqzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wsagtnon.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zfbfznrs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bubfcaqz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3elztaiws.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qzjsjbxl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3nfjsvqou.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3twhrfcqk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ummffezx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nljdfgoy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tqjqhshe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3yotsadil.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jakadjqu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3weiocgjh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fnxuntxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yqmjwbzj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3iiqutciu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqidqboq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rwxibpyj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gnwzxxse.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bfspvpxd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rexeghft.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dnxrmvup.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ymofolyp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lilhsrja.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3putilglu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qyimljga.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3tkliyfst.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mogidwuk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hxnnjuxi.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nlarhvkk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pswuawsg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rtoddcqp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xpzmkxys.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vpwrlhir.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3bounwumn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uironeux.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3wdivqfji.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qalsnnfy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lawzlstv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3udflcpjp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3coppybiz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lrctgpkj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjxtivf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3abkoblmp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdjtrmw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3onteiqpi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3cdtqkplb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xdtrvuks.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dvduglid.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3tmelkqwo.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oefkvocs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ksrlvpmc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3crmhtewf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rdmohynb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gruedckd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3ufvvnjsq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mncuukwu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kmjwkssl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tdaekwml.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3tskfarhc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3nflghbgp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pviuytst.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qikmrfzx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3eoztnwhl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wozpyans.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3qizpblhu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3yfprzhgh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mfsupjdc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vzlgebuv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3msvkvjmr.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zfgldqvj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pxfamopq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wbgksjnq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3dcbpbxwa.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ncfyanyq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3dpaxsbaq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3qatcvtgk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3fzhbhqww.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfrenae.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3llunlvaw.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3axfuieij.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eyzkxtrs.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pslvmyhe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zmcxxsmh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmvvzhr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3euqepywu.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zokjiiwt.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfjvuwyr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3owwninhx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3cabbgynh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3wvukvitv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3efstgeil.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3knnrxhnm.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3uujheycd.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmqavnsj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3izbkkius.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vxytpjer.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujtqshxw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ylblwyem.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gvwvtocn.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qqtdexhr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3moiudaez.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nhfnynwv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfrfndik.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bbcsssbn.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kybynnxs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qsdynchk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vvdqnmab.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3lrbrwixa.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3exlnoioy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vzyzxjtj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3lznwwjgd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3umrzhpyk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xbrpouxf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3qzinxtro.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qkldfzkb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3enhniyrf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3fewlqxor.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3yurlubnp.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zuhxgxhz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3quxgqxyk.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fmkhmybi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xbqzounh.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uvosqxjy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ynjwnahq.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3janumckp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lemqincc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xvylgdjc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jomerzxr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sulpgypu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bdowljyv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hrqbzegu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdbrvhs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3nrwmssad.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qbuchzkx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vfklkndo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wqebugew.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eusqlgwu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ohmrmniu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gtoyxmze.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3cmehhfpw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vittksue.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3taaxrfrs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mrrfwojd.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3pscxzzwk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3zqbxxupx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3mamvwjzq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ttcgrugi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qwbchdyf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rsvjyjej.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3qfqufche.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ldbobobe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nmcfexhg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3vgvhgmjn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ibylsaes.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wgsqrhur.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jarhmsae.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3mumwzrdm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3hrascyov.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ayghsrkm.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3scpjlzbz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bjsuekbb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3plpsfxmh.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qqhzuypf.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3akypoarp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zwtlqonw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3furxzcrn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3emcdudza.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nquvkwba.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3nhuosqij.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dfbnjbcu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gynmgiqz.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ynslrblc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vfkaygcz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xlwvgxcw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3uecaxtbb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3xoajawor.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dbcxjmne.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcixboqf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bfyhddro.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3donoigqa.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3isguipol.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3cjiervok.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3oibbvrpa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwupcr.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jwtmaujh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jwskjspe.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yuoeodro.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iqhmucat.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3sfdzddmy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3druhpgof.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3djgtdiic.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gffvihpc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3oeungvjg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3yerfkbcl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3bzliianl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xrcpvnaf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3aypzvifc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3dcduuucu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ukjjragx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3tvtdvscz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nqomsgpc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qlamwlfx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3zztixkkw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vhtbrvpa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aojbzorv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dyoafzlw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jjdzkdvd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3otmfxgss.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3awzfypnd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3kktebbcu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3vhxqtvsv.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3frqgzcen.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kkxfqutv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ojzuqmqy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bphuuszg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rmqhcryx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mmtlwyuj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbrvmkbv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yvzaarpx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wnmmdche.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3olcenxba.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahphputl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ddfvqbux.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ucohyqfa.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3brrzgbxc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uflrhcaa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fyzyilbg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pssseueb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3oebvdgwo.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jmsamyrk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3xazwzfie.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3grydtfxx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3legwtnfn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ehrpbkco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utvvfqir.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tndznprf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwutmpgo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rpzjhxtv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3asbxgkzr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3sxpofvoq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jsoedfkv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mhbaiyyc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vpcsykkw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vturjida.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bawgerkb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sckfmivm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hgogwgyp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vtvlhssr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vdpusvrn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3yiyrgrow.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3echiyscp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3haphursj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3qnbwgeql.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3prqicuaj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3fkmdsklq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ltotymda.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qjohjmyt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pgnrpwlo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3saokodcq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hdayslde.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ydyuqlkd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3rmlfncij.html


<!-- 参考信息 -->