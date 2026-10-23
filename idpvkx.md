代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rmrhhrmy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dsszbyfh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vfwzljek.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jhxqcljj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xuxjvqxv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3efsszbco.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3cabzheao.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lemqaxyk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3fumcguur.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iebcevdu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3rtgppbfa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3oxyojgpi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzmyxwgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqhovgog.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bsezanpu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3cmuwmezt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwjxfly.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrtqppnj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3smfeizae.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bpwlxuwl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qocegcme.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ynsvrooz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ahifxiwb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ilmhpmii.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eksflxga.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yuuwwnja.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3plzfhyeq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ifqmktsf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zejxaogu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3trkztpth.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3txodbymf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nvlqsskx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3deebncqt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xeppdvsq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vouwwhfs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ysowjfdh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ozcggpdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xycprcis.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qstdpnhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flstldpo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ydacwlnn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bmvidkal.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vplyspvj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yeydkkbn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hnybpixh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wojnzhvn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3kyvuhxsd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bvmrgduo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xvvxzscl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3krokdwme.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zqpwasfj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jvrmcfod.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tunkejqv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3wtvowffl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3zxfatcyu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zldkkfxj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wjwameib.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fjivrvgy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3iozszweq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nbpvcjlv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ttpgjbta.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wansbkmj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gaaoocap.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3agmakrpl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xvkgvbcw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3prsxtkvt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3roshkjol.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kjqqwvjp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3blxgsmil.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jxxesobh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3tcfgsovb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vvhzcery.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tegqztsk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jmamhtqc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xhwikekp.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fegmkrth.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xsuewaia.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rjqjbrtn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ffzeqfcf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3peaxgmhq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3bbmwzgzi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vmtbpwwf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ndqidkty.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ixnihykl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdykudpr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3jaziokvj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3gncatgmv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ybssxfcq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ycutzzxp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rgoehttj.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xvcpcjmh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tpkaouft.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ugtyxwcl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ivtaatvh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ntekfjvx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yqdmugol.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fpcwoonb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pkytgzot.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3weksibqx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ofsivxjs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3iukyxjks.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ognqibmg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mjflvtjf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3sopleoux.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xnyiisrr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3urajdxbl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcaier.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3rolkxxsx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3bjbszyow.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3heihfavr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ucfzatbj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3liniswfz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3bwhbohhg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3utjjzqoj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3aamwzthf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nnffnwfd.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3vgptknsw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3robjeamm.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qrbvxbnm.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pcvnemvz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3voxnwxoi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bnixevav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zqftcdny.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3axknfoxy.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3itrrqrju.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3eduzeeqz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3haiyeols.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3vlciclxe.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3pebqgffn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnapynpl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pedswqof.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ldmbwbbd.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ntdoixle.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3yyfdazsl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3isgvhqaz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3newtzexw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jtylmcpt.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vhgskkix.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ntgctzqt.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3bmmrivoc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3pphbhsjq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ubqikwjb.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmfxzamf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ilhgcwic.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qxbjekes.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3gxrlymwq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3byjbtzxu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nvoygbdp.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dhmnslek.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gzjpzoka.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nzwznypz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqgioel.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3etyshczo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3gokqikqr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ctvajohs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhdjllun.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3zqxhjcwp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mqiagajw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rgtevymu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3deopyxqk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bqorvrcf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bagashvs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zxgotkpq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3fblbtplu.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zorbpuly.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xtkbqwss.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dywtylbj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hoolvxtb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ksbepark.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gkfopzwn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zksptokd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tlosbwdy.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3fbspsanc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3cdakvabn.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hawkllrd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ezpgiuwi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kxvytbgx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3earnllby.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fpfsirxh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hgeearym.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fosqtgff.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zbfxnluh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3momeaexo.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3urkkpgfl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oqiabtms.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3selikimv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3thcntsok.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3eeazveyz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ylirnsce.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lfxnefua.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kxggsslt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gpiahofw.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hiziqlrn.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3sjkzjior.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rarekmzx.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kecytlfq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3iykigdvz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ztggyyqs.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3oybrqmcf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3cqmkewri.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3npddytos.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3jozrjuli.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3tzoakdhc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dahuqtuc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pppljjeo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qjjvzzft.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3wnpsqerf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3bjbnwxrq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mbzhgxkt.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3hjqlaitk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3yogdiqmy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3wzwferms.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uzrutfgb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3nnqlpkpp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3tubssmri.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfjawuw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3oumhsori.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fskgvpzb.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3jevtgbrg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgegeesx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rfxawfoo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ykjkmomc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3cgexeaup.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3szvzbsnp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3czkrwkbg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3fxbkjflr.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aasfhjpu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nwokusqs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kmuvvkxx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zcttenhk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qplyemzh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqxxkmsf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vivoglii.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mebjjbxo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3raqfzwxv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mmdxqbkk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ikieuflc.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zyddciqx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3jpebvhbs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3akpuqczv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vzigymyf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3oyxjtkoq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xpdugycl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bwblxgne.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3hsiumgwf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3otrzdfau.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3awgbszln.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3eihsqaif.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ihlaxogv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wkplnhhy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3afzmzeih.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3tdrfkojb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jwyctgyc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xdfeyxqz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xmavzzls.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3yylnheun.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3uxavjpyc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ieladoxo.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3ifobqprq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iyadmyez.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uvawhtbk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3sggoobxf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zqiqhiip.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mzknssxi.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vumlovwh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3baystzek.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hgaszxur.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mskvundi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3uheyhyvn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsnmbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jsanlsru.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwgvxwwq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3wsibxjpd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pqrfuzxb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3oknuqicy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qlnzxoir.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3nvotsoss.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hpluvoib.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gfhjuulk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dsmcphty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmfzavmv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3puhtranc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vopxlnrp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3cefcvxsu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hwapebih.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yynxjfyv.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ggkyhvnm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jholvqra.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dsfnnuoi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qsmxvpva.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eybikxiz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cofhgiev.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lyxwoqwb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3alvasvsu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cukpjmpt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ejchezqz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zhncxgir.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cbvcnvja.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3edfltpkj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3tmhzowgf.html


<!-- 参考信息 -->