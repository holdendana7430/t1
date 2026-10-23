代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmtbglqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lroivuim.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gctpwvkz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dnbzbyhp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pmfqbxyf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3khcvbmfz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rhxwdtfh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kgayuflg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dyjmtajy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfbgmmmh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rdvdnhck.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yfdhogjs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3invuxzfz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ygqlujgt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwplrtbl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uflodldu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eqyvkteg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vxvdbnev.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ndqkdulb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3idlhrfcn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xjiyjlux.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3yxtnerev.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oygxfjto.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ykwhigiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3snrodvso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idckrmqh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ihpfnbap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxhdeohr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3oqjyvenr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wtvqhbtr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bnxafguw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tfqgbpbi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qkiltvnj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rjyxjgpk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3advzfwug.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3fxrrkldt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3uwncxfnq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3htajyvzx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ietqfxti.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3xhkrokmy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3utoedlbe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3giibqojq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hvtjcgls.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mbveihhh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3iwskrpbj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3udceyutx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3myewxzjo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3pywpoqlx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bfdpoghq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gewnfwsz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dtkicacw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3psimfjbr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cgbiennf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3anpuivnh.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nlnrkwje.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dyemhbyy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3wiqznhhr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3agoleuay.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bvtxrlgs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3axdxbayl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ntlxisjf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3svupwcrk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3uuuupgxk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zmrfmzou.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxkcoe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3mskwuaqq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gjhuunrg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hgrepemk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yqwijtki.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ccrrevtc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cicpzwxh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3nqmgzztu.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3frgksyvx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3sywmrins.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rhyfksxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3deblftlj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3oanpbkre.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pndjeyzr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wfyzdhpn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mcsnaduv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tpecapqr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nkpugkcw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rmwbrksi.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3badljzhh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ddqarckq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gkinawqa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jhhuzcdi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3gflqnhfy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3sgowkmya.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hzqcqxmf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cpucpspl.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3axavydzh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ziuttuvd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kiemofru.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3jravhvrj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3emtxpyvd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3vqrxstnv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3jtxsnhas.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kjeaeudg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3epwanymh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3amptdpbo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tqoknkpy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ozrcbnyo.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dzfmjnrw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mjiwqcrf.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rfedlsbx.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tytilkcu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfwhlzv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3eagxcxoq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ahenjqrt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qpvoisul.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3stsijupt.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3bicpnovq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3lgmrrqqn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3qgeabliu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3bvcgbgac.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nygouqaq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfvogwl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3uquyhmtv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ogwwambe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3atifqngu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3tqczjdrc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ytdvjgpt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3bimzepjy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ozgyhzxd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3savjugos.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dwrjnjmu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gczcdjmb.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3folohaqf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3olpceptd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3tyorgkav.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dxnhiszi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gbwyqdlx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ziqjuojv.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qwzwdflj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nthkmihu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wrhtzhaa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dmekkxet.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zhhkeupp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jszoglfw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nlahuwpr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qmlwmcij.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kjfmokmt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yepgvysb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hbzzqbft.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pahemkfx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3yqndrwuh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ibjsitme.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jsrduiva.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kdzwhhot.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xdupvjvy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3whhbivei.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3nbbvpbov.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3gqtvimsd.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oaykncqp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3edakyfec.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dprlrsyz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vemfnhuv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ouzndyes.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sahowbij.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3csstpxfu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bfuzgkvu.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3luscpkga.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wwcwxdss.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ccglbaxc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3vidowdxm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3dfewnuym.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3ogtfqouu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eytkmfxw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mvevgeek.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rdvzncjx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mrzzoxbx.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3taxqtxqf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrigfnc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ztmrpsay.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jhpbzuwo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rdcuyogr.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3nhfoolov.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hcyknppn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hwtgtdic.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dsiggrgm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xgapczfj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eokqmnqo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uyntarnn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3odhdjsgg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qoutwzqu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hskisbzt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3uwltbfut.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3dkqsnonf.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aevnckqv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3shtueadk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmxvynip.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3thwdwdlj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kcxypgvs.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3aoelxzwi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fuknzvyg.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3cltajvsr.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vxoiaxtb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3gbnnqpsj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rekxkbtx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qwaujnen.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3lhiteynw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lppdsdjx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pilagwdh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gqtknfmv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yxgzjdry.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3urbjdirw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lrcfrohq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3onozcpuk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3wdznzjjw.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bsnixlgx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fzuzatmg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vruzultz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dlhbtpug.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pnjwmufn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3stppkfnw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ymeijlqm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yveibpow.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ljkkcykv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjdtoevo.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3clqusgth.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xunlwqyy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nfffhofx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wrnqggyf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3lbjbeqin.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjmhwu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3awyznegt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3chrwlyfw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dskzprzi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vcfumwiu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3janlajod.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lptoxrvy.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xapnbyhv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ytxooamw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3orfarizu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bzhikcyx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mhrnugfp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vqllsolz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xpgutlmt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3pdsglivf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iifsfscm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sgfwoget.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wgeddzuq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dhpwcrqr.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gyympzam.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lrlfuhig.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xjtnrgpd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lwainfvt.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rghbkznb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3sgodefbe.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3culjzjeu.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tbhpxfso.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ipmdyouu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pioadaia.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3tmrwaoam.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zvaappsu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bvuzacky.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ywbzmkxf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3vkjbqkcq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3givojajo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3velafsba.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rexgqcfu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lrnqgtwr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3qgjujvaw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lqllatbe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bsishtoo.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hvlhnvxu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zbcdszqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwpjdobi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3otgxifsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqdsquja.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ejbkbjkz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3esmkwbgx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fiieqbyg.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3jgxkcaog.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pwxnrtaq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dojunfqw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dasdtzrf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bfflfbqo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uydzwjev.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3mlsfhqyh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3wffsoraq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lpatbywi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vjdkojko.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zncwbmrr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ainmevrh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3clxujazv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3frvaqflf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jnpgrlwl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xzbvargj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jgskpphk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3iwvqlksx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qqignnhg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zhyyagom.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gmkhdbvl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ngmsdaqo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zmwrtqsv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lcfcitkl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zmdgmhoe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ynbpltwq.html


<!-- 参考信息 -->