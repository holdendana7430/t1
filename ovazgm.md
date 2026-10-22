代发 wailian999

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gmwhhmzx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fqvuuutx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2plvcmcdk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlaeoufa.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehbuiaep.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2toeprazu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xtfuochw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tevlbict.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nchuoplu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rskxgtlr.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kblvhebt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ckuketmr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ckpdcebr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qoiuocxi.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbemwmgk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qonyeqhy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2uvfcyzow.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bxzgyrix.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2borqsxpp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aeibxjgx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qsjcjxuj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2iykutlny.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ynyjvwnk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2otcbyfwt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2skjkaway.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zfrqneqr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjrvjmuc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2yfwowmvk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ugjvkxrh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qyrfxkcz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfnjzuh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2utwndshu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ivtjniqp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cmizrdcm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wculidif.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hkfhhdwv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gxcnotnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awziglxs.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rihblwvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmdlvkxv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ikqeawln.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2bwjerxql.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2saoygkpu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pvcfgfpb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nzxxuzfl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ydqyhbql.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bookiphe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dwbcwvzm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nanklgvp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wfamlnhp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2iahvidnb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sudnhsyi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2wgxxfsgc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mttwajjx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fogqxuom.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xvgrqtfq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bgsotznf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gsuszean.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkjlronw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2xlypskyf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qinoeavi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxnxdzng.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zvyxgzyj.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxwcilc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xjhwskpp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fymorasb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2twturbde.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zfwhxapw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jvjllkgi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qecycvaw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tyienzkf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ibiotthd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rjxxjnnt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpixhte.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2emogyvav.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2emeumuuf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2opybxbqw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zmhfdkfb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2oidlnwdn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xesdkzlr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tzibwnnz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dxbpgilj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zbcfcziy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2qpcmydjx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2luvukkrd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vvnwzrwu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2olywvxre.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcpwjgy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2hyppytrk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dagtswif.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nuzngpnq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvoodxg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bwsyjpdc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zgkwdujs.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pvjogxxs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2siztjkme.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2tywdsjwm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2makrvcjh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2mqbqkbvx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ywezxfev.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vaokocyq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2ndzcksyi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fvfuhibb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tgtyaxax.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2wkjcdvwn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sxwczpqp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oyzlzrfn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2loefbooo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2qubakyrp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqatsfv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2njwtuboj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yplcrrlb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2efgqatby.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wotuixei.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xxhxwxiz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xynbctnc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2eelqodbw.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2rivelccp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xjuehprx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2igakpuma.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rtihalri.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2husbqkyx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2oqoswqqb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2uvbpttnl.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rndznfkr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2oowfqkiv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hvmzudpu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lqybszbp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ntcfrrlc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wdtudczg.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ggpxymez.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2obfpaxur.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vtfiicuc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ambttzru.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qtasoxus.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2mzgaiziu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2onvvzoay.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2nxmozejx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2ghnstvjc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2fszkbytv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pdzgoeto.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2uuomexim.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gphryerh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2dbtnltsr.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bmhyboes.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2sfxodxqk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2gllcgkta.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2gnqgmbrn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2xhadzpex.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ipnieghf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ypiyrbnk.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hhgszfss.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bflxoysu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2kpkoodzb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2qximehyi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2scafahfq.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rtraljeu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vhefzdoq.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2muosspfd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cjqdtfuj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2surbvesx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2prrbuvho.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hcbjuafa.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2isoxjuuc.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2szcghgja.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2tslpdmmo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ebkswzzt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ikgnljhd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2oloiklix.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftkhstxg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2gsflaijf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ofbletrh.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cdaoztvq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2qntsgmqu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ubqlioub.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rbeyxpke.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2eplzyluc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2arcwqmus.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ujgwjqfe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ergspmsu.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ohdwnezv.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bxelsupr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ykllygbi.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2clcbiofa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dofkciij.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dxwjnbmh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yddjfukf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wigmahxy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vrreneve.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2pphwcwgn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nldzxvqy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2alljikrz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2agosoegt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2neupbbjx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2utvedudg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2enguxqjg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2vapvlazs.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vaoqwexj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2itcsrcwm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2cojqwcgx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2sciupveq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bgkthyfd.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qkzrloao.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2xbpeblfz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2jgspzqts.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pzvovlbe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2stesowwe.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2dpkugsgr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2mcfzngfq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2irjqgset.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2noedould.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ckbivzhp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kzufiosg.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rgepioyn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ijvdocnn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2znfqmrtv.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2coglybzm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kxtokmme.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ulxenbsg.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jjdohuyt.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vdaofjbc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2esmbsouy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2eensauww.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mfjypfym.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vkmkyhib.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2uwhljqhr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vahpovuv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dpnftkkd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2strfalhm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pypbrgtd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ausxglzg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xzroksdn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rvffkgtl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fxntkxnn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cpstnvdh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yyecvewh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ydbkibnt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2frcdpoua.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ckbzvbya.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2sxxzspru.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ljbomwpl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2okfudjiz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ahlzllxw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qtddiqdj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ahczoqag.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2jxuiakxo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2olfopnhl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2woiyvtnc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gjnsmpau.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rxamekkl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kdxdbfro.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hbgussfo.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dgzwnvyc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rgorofbp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2zljuwnii.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ymunbhoq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ydwmhenn.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rxtfqkhi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wxvzxxuz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2craqpmct.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nzpvvbug.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jxlnzdge.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vakbcszm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dkvqklng.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nunczkpd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sqvnzldq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2coshjxzu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vjlupkpz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rqgrlbsa.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jkxohfdk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ujzmymti.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egqqfgcv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2elviyvhw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2nscaymls.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rzwhhbqw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ceizbwll.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2geamwatq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2yimvtuxy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ddresttt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zwdmximl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tusvgano.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vpowxlsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iptezjaa.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xfpoeaaa.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2tubifehc.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2utahtjty.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jpvcvxey.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pfggyolw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wnakkfcw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bkwyouyd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tlumpsen.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ywnhlckp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yljagieo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2houbfbpv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2nvqfumyd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bqdouveg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2spmeqanf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ebajwgjx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vgderglk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2yeipjfbx.html


<!-- 参考信息 -->