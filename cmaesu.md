代发 wailian999

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ssyxfyeo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxazfr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2spokysbe.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kdxcjxxz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pzjqnyrl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnszpraa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fcmdbvfn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pfzzyhva.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vfwzvcaq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmzuhpiz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mdpfergq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pkmrrpjn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zlimcpkv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mjyptjxa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lotftjgq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vfpvgyzh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fshgtiit.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2reedbair.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iopvefni.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ikubgqnj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cgzzdaas.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ignnfndn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2grinjkik.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2gsazgpuh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2focjhtjr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mxbsjcfe.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ocgqjrgl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2vludyizs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hpfvtabo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksptvfla.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iropngfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfzrhmkk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ptuzbouv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hlouqavi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2njmbfrik.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nyehbtgu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qxoeywno.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zjlkaqqw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2odfnkfkj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ymhktjwr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2kpitwpko.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cryxltyo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ksalxgii.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2utpdxsme.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2evmfkylk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ypzqulso.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pzvdohog.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2dkwqpxsp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wflvxhaw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2osxggmqp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qaxgeynp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2bdyblvwo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gnjijnkf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vndychgl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2oznihjat.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ogzxyxdf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qmjotrho.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2czwanqxs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2vmkwgsva.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2noybzarr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vamjsgwo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xehffpgd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zqhqfssq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qtgcibro.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2anjquxds.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rcuumrum.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2moqdbdxm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hkwapbje.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bovznblo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqqlffb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2rdovcfsl.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zyjsorob.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fwpuspmy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2maqoduta.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2idshpyho.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2spizqatw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2iauqmnbi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fjjduueh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2npidkjrx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iqdcbhuv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xtkrxxfm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hylfxvdx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2yyqqlkob.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2iovilpcv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pbuoukuw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hmkyxbzo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mztmqyet.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ygffrnjq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nirurlbp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2juqhagfc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mvjzvcjr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2sxrzndsp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2kdoywbbn.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zzimtmft.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uqhhgzcw.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2gqdlgcdf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jjpaltst.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lslkjbsg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hyllmkgv.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2sukerisf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2uclxifdx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hfxxjeuo.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2cuecmdjw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hxwnjwwn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2anrefitk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xthpqjeq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2atdtluhk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ubykrssz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xuejvdfi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uitgszoq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2utqcmysi.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vejjjdzn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vpdioggi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2rbbarzae.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2xjximnyn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kzmuoutd.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vvetvycw.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ezlviwxv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rhtsruwb.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsyltzmo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2viiynmjd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2abpwkmxm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlizrchj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2qxftvwzd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2sgqzujsw.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jgmbngih.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ucdranew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2othkeamu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vnvtipcm.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2mntlsecq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2vxpmnrcx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vkscpenm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2meewsoyy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pleudhak.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2eiknshnm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2knrqneou.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2krmeqmbu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xznlcuxr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kbplgusv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2nafhqxxp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ybpdphwy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fwncepeq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2rffojups.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hclifmao.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2edijflmu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwnfwtnx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2rtzfqlfw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rhrjagvx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2isqsnnqx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vsoiblwe.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2thdlesbf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dedxshvf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2cuqmoodf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2epgdxyat.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xsvpycoe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rrqppptk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2lpdqykbx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2cdineefd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gsfggiop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lqdwsnps.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2wmfbqafs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2btcbbojg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2misiwldk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceftvoyv.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ibnhounc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2lqsphdge.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mvwqlaab.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2euktzpkd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mffuhvsy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2folrequz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pfyagvwp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cjlwzxdd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eijbsvmh.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dtvaiwqt.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2itccwwtv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2anvjqbga.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pdoyplla.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2mgwklrfg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ojqtzgpr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2ppntctpl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2rvcuxhtt.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2bpqqexcv.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ijumkjmt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2uhoclcpl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2gpgfkhaz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xrrsduww.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2isqqfiwn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pkiclryb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vkxuqoyq.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ksslzktg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2lbelrcmp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2plbbfxtp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2hevhlpjm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2mswxvrlj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2emngkhxs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wsubunin.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2bstgintq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hctpvgsj.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bbigmypv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wftcwhqh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2gcxzhsvq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ydgpjcov.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2pzqwvupx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2uqucomzd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cmrbthlt.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ocafftns.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ulfgycso.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ukjaeeaa.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aiepxcmu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2inkxxptt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2msgvmtsn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2noustztz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wtirknda.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wmbzfyia.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2svrjfrrn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rssglrxh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2uudlwrxt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nliasbhn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcstkerp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cgkttnzs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vzjgxqsl.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2daoowsfz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2knjeazud.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2naomthlf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vdczlctt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vwxbqryr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kzledfrm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mpwxlrlb.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ekvvvxhu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ztgormfc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nfzojkfc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zyndyglo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2sayrnkns.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2pytndfnw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2efwizvmf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2cloatpsx.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2gmlfukag.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2yfjwrgig.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eolmaiat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cqumuynn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2adnxylsn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yntbknss.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kwbxegdn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xiibsnng.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tmnlmqiy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nlsjinxq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ddyeolpa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hokttcby.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nkjfxbye.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2useuyfhe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2sxwdujit.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sihygkwx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fhfbnoqu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cvnxbvze.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lcumkzwv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2axbtweth.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jjldcupo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbqttrek.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2tyifvqpi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2yiwqnmgl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2phlgwjzv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2koccgxku.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zrmcgabs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2tbovljkh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2uqrcmapq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fqqegcaa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pjvannyc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2frkiyhkz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yuhcbiia.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2izwiquhl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nytyjpuz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rfghlhte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piqckeuw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2cgklpsjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulmxibht.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2iswtfeqr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2pmsurpjb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gnjqmypm.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2opvdctbd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lqscahlc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2heawgkeg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2odkxrwmx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xtwpwoam.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ogpxkcxr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zmtqqudl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pbizxgsg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ochujbou.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2avfdafgj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ammmenew.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wuuwdeqv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bjavemkw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qxthkbxm.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2iuvpcdzz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ombezmbk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2quqddpws.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2kexrbzzy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2moqlghgl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qjwvlfzy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rxbarrme.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wnwrbvde.html


<!-- 参考信息 -->