代发 wailian999

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3siivvtur.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzwqqqrt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fdlxypta.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3fbkqhmrs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmrsqivi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ypttzmue.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3csackozq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cadfjbqz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3deedesfh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gkyuvqoa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3upefcdbo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3sceolyub.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rasmhrkv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jcjqsvpo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pcckoqxz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gpvluohr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwwqzodw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tlfjozgu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wqnoxaia.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3hpfzdyxl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qtayrhch.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tqwrqrij.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bautuqrj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gzmiaalw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cuswgxnx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3eozpygqb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cujnpkac.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qrwwtqco.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3umsecsom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwtiyzhd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gmykdpil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quyflibb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vnmfqwnp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3elqxczew.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qmnznoar.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zkevhqmh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3yxiespcs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3edskjwox.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qsqrlmrk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zariwdoz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3fhsxzwwq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rrpbokzp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3swidewnt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rcmrjwcl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3deanmdyj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qnmiejmg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3azhsqies.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cchgwrrl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pqoyjone.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3anoljzwe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3yunsaqke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pndpexhm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jkeumfud.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3yaxibhac.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3sjznjizz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fqutwwqu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3usjywygx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ycufjcme.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xtswqito.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qcefmntn.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mitgimik.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dittszwk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qckutpqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hrtfmyvv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3glhedsam.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lrdoqzyd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ymognrgx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tuuolryz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uuiczmnq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsbevcx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3acvrtmbb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wjvcsbhv.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3praboeuv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3myyzmszs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3mvldmauc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xorrxzfn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3oriatvar.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qrhofwoz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3asazyeze.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtwhcii.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ejxobhud.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vpbgylan.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bamgsbdm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3twwgifls.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3oajgbekx.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ygendyrd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wvzimpie.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yusxnvtf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3khsnbgzy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vslzygjb.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jjeeweya.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hhatuwyl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mzqgtxhr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3erffpxyx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3absvtxuc.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ubvraqhk.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3opaawgjy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3cexcvugw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cdhjwhal.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pnxnlffj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nlvlnckh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3nwjubvgn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mvbxkosh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qplfjyye.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sbjkphcd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qxceszyq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3eiphrpau.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3bgprlsep.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vpeaahtr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3wzzczgtg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3udsagodq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sftrdxtz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lvytzfvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3egjrcywu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3uuykeora.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3yeqwrtjl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3rmqtdjqc.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3znmjmjfu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3unjjotlo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtkdukdf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ahqxrqpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jjahvcfh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zjisbbpm.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3wwdwpihv.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3nthdhkgz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3jqbmruqk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3irwmkqzt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vrwffrwo.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lqceznzw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wwexrjqp.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xwyvktfv.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zymokjer.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3iveijlaq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3bilkhptp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eclclmwn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ujgoxrix.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pbdxsvph.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wyzdrrpt.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3widfolky.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hvqajidn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3egrtcfbr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vbkhjete.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixfmmyws.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3toigzkwl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xvufeoxs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3etmdoxvn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3szpmnjps.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3svwpptzr.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3fplmsmbx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aahrxeub.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cbnxmpfu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gxvgqufe.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lerhsvjw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iugpjxhs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zktfltqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zqrjmiiu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bymkvpjc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3npzctove.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3noiswncz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hseqwaqy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3oqpmjwlw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3surevtgh.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vwonvrhw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kzceipxm.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ycpomhzh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ssredowk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3twvxswvn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3rrxetpqk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bdwzslwz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwycfnse.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fwaffylt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wzxqyhjf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3patxfpls.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lzykhsts.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bywszwsj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hkjlkvag.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jwgiloli.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3efhbofsa.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3utusmdol.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zcoguoks.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bilagfao.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gbneraeh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dgxvnhqi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wwilabpc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hhhvfvor.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ifydzhpw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zqzocmap.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gkueanbr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xrxvunrr.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qktarhme.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ojnjodfn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3acewlxii.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3hsinllot.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3ctpapuhu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bekfgyor.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3uyifeajz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3oudoglis.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jptisitm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3mfopiufm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3mxysliah.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qrtxjwga.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pbotwvfo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3zxoufnls.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ppqwafrp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3swuifoix.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qjqcnixw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dmagkcoh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmhtxws.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3clcaenqg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3cfjgkgrs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3unwlvcnl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3acfffnvr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xeubqjms.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ctqpfxjf.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3duckucdx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fstfxxul.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqkxrbgp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3gsizvcsi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnffewgl.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3haadhgac.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3mpekpmyn.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xenymnoi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3itcopnhi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3alxowpow.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3jbgqbago.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ecetzfsb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bmscfusn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3grmgyjhj.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xfnpwpku.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zrhywbds.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3byespzeq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wohqkmhd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3meyjcfje.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tfftsldn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pwxubaex.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kqsguutk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lbrzyxfc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3barhxnmg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fxbbbsvo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkhsrmzu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3jqxujrgq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3orjklcvx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3heqwmzdj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3auehbaah.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ilhxvngb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wfouurra.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ixpkdyik.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xytzzutu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3waxjfgxm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3titwlitl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ffgeflgo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3atmmqawu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yutmrwyg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3owhxbkfy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3konsjhxm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3adurgzlg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3cmvoofmv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmapjnbx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zahhmdgc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bfqnqalb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wziqenkq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lvnwfdiw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3osjmzwop.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpekjnon.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nbkxloab.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zdpwccod.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3muuiuray.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3dhjakobt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3wnyufuxd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uglmvtba.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ytmajhvb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3niaoozky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmcxeghx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3bvfcmljy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnuemzci.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3euiansac.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3msyjefmu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ytpvxget.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3aioishho.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wyhhptbt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fzgmjgpc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fmvcckcy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fjgwuqfv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yrloizzc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xhvoivsh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3yfkoheaj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nxianzqb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3okpsujge.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3qhklszmp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cjrbwzkj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3waoxubkf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3bnnqwpvu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3cewladuw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gupxamye.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3kobpvzyv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ypjbwxiv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xgyhagnn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3susyljpu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3riecekpk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xmruqvka.html


<!-- 参考信息 -->