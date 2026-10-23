代发 wailian999

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3lhoujtdh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pyhozgte.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dnrnpirx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhpbvyf.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kspubauh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dtgukyte.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tikzjyvh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rmubgaki.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gacnczku.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lsbuxokn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yikcaoqk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3llcvuoov.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yyqrvsus.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdcnyshr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xprtirzu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vxjukikp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hbywturc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3eonlyssy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3avnkrdhp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vtddfshl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3awyvdeml.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lxdsbikb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gpflqaxl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3egpsywnj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gbpwirrd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ohaseddq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iryhfjvf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3awulvdtb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3udzmxlqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgnjahif.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uyalvznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rclnpmsk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yqkujqcj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dhxfybwu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fqrstinz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3telgwyqf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3wucsgzcz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eyontvug.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3itjirscw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rbkhynir.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wsekldtc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3otmcplfr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lqxknkhn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3msfchzbz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3snzicnhd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3axmkmiul.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3tvmtdsnb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wcvpuryr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3mmsnudnj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwkmmfq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dsktbezy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hcxembih.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3hprqmelr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qbqymyvl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3kbegftho.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bwwqhyvy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3znbziirq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kkcagnha.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkyctugy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3sdnmjeqb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3fknekxhs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bgidxfxh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3lwwmzive.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dbznkfur.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tczkospc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zhumlaun.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3kkoxpkld.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ddqzehao.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ojhyaeso.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oguecjhy.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yodsozaq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ykwelbra.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xqrgjgbi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rgeoyvko.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3icqjmohc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vjzqretb.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ijjhqsik.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3usrhiqhe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sqtivslo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nouclpkb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fcgwsibg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpobpjt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3smxmuprj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3aposbfbv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3csamjhne.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zwavlfmp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3frdyeequ.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sncpbhaz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xwezahey.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3atygfhja.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wbxvovyu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvfkpte.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mtacpdgy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3vpjomqfm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wvrlgtde.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ucvtzmse.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3khzpvhvz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3oibjahrn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3mlyilxwd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3uhfweshn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3cixrgwjr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3aivggqeu.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zvxlqkdc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oauwqnlw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3tuvornpc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3chrkghkq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qxltlezc.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3wwqmnisr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3etijkczq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3khjjtrcj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ndpftbrd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3luwghfer.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nryjiruw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gqcpdmiy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ndqlnnge.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kzeynoyu.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3inenlwmp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3kfylkqlg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ootsowta.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bkecjsqm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3knjupvmw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lzyqvqqt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zqfhwhah.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3coxwfmqr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xydxzkuv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3zfmtwcrf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ripyrvba.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfzbwtz.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mutzrxwm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qevqniuv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gzkeqdrx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vlkvqqle.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kynnwcez.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3vhpwxfie.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3dovllhju.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lybymnkp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3twtoxmjj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cyvmlkjk.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qwboaxzm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xpfdsvse.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3szwhtkzm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fiqyhwai.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbjnmwio.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzezsnkn.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wpmtcpoi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xecnlgdh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3qbcovdtt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dreqmeyg.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wjajsjci.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pbtekicl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bsuwngfs.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ujcordnc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hsolorqu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rqjapqhb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wupfyfhx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3jotblwtl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wpeibowu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3yeiycryd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rqbdfuud.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3qwbfjzhu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sexdprvg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vkdllerc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hckpebgy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhmeebda.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3vqjmjwcs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3mhgpxffc.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qmlpshyy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3qicawnfq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlirzgan.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tydgcdqx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kcaxoxmz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3avhwywvg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ywtsltfv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3viuejlap.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3skqkjyfe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3logabziq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jlcqmwmc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3glnebcwh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ojuynbym.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cqaqryzz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pyoqyhgu.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3aqisanso.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3omtmharh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eyrobmly.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3arwwprnq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3orcylqge.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3cwjexenp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zlnozlys.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tsdxntkl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qmosqbtz.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uyubdyip.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ruttbwgh.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zxjjeydp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3roksduso.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jdvaayzz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3gkgtcffg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cqvxyeel.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzgeqh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vbmpwxuv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mouybwbi.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3nfobqisf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3wfyilpjh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rvxjmpcw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hpvadgna.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nytgdmac.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3cnmocmtu.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3reioqvqa.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qauagwrd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3duswmxkx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yhttsvwz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wzkwqgpk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zlnlhcpr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yzdiewdb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gybwlyvi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nniqovwl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ueodbczw.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojvcgsqd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rdnmokfd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iijvnwxo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fwxixhrk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ipnknbes.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3klvsnrew.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bjefjxes.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qislheea.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ewubmkxc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tpxbqszl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mwmnnqqy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3kgnpqloj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uwvofnpd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3qkdvcfgg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3noqikmto.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qagmvdox.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3juvngnsa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kgikkvwr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3mbpjriov.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cqbarmqm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3recfmzci.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jmovulpo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3zijvvdre.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bhckjlor.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3atvfoidw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qtvifetg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3szsveikb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rngiqaaz.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vjjwxghb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zzyzuwoy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3riickdue.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cafsspmf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mqaqnunk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmsstut.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wkmshaye.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3tfjplocj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jfsucafu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tvnkqehy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3apptaizs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jkoghxkl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xhdrlocx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ociddans.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ngncbkie.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3udklmkap.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tpgjodah.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yxztaqvs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3woozdlpa.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3keiuauav.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lqlrdida.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zslgzdem.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3herldtlm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mhfaexhn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3znngrkbo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3exmhttyt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3npkbufgm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jzqhmzhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idijyovw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jnzkrzwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npwxwpxk.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3atglplyl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3numikjby.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nbbudsgf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fktwlrqu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kdvdwzvr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3psjmscoz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fdnlivch.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3tksgtqfm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rwfhgmaz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qflsyypw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fmwmqduc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ckatnkqt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3hconvkow.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3uvpmgkph.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ngqpavxo.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3okcffsxp.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xdxofkdp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tefkykum.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fgfzyryu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mdgkwcek.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hjyepnqh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xdqodltf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3qmmxjfyb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3adzrozji.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3djpnaaty.html


<!-- 参考信息 -->