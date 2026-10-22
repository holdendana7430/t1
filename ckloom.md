代发 wailian999

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zhhoujod.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2gkrxniem.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nkirwrsn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2srdfqtav.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tfstypfs.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xdbquowf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ujzpzall.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2divvassl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jmfwhssa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yoejksfm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wjikuowg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2qjukmchf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2rljowmzm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgdrazkj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2omcxuthc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nuuwjgui.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rnjyeles.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ejvwaetx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfhsfugd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ourdfdva.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnuuvolo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mlzeojbq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uwybsdvm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oflfliud.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zfzlzlpa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ucmpmcda.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2slxasdrd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bmlgzljy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2njqkxiyi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yhupdprn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkkexty.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nkxnacsy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tugmpakp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2knhzrxvg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dkrhttei.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cvcwmcbj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mgqlcbhp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2frmnagtv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gkenxnif.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tkjfdchr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yvznhomr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bazafzmw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ylmatfkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksuwxizi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cwllvfqk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hjlefexu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2arqdcoek.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2tgpfiaou.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2gtjtklgi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2blqxtsit.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rhozpreb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ifqzhwvg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2wtjodvln.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qfpcndnf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jptxplye.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2yujxqzst.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kquvnqyu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cbdwucyl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2unxhpmbk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2yucosrkp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kpnvyzzy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2djvepifr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2tjtwwthk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2myezhzmz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2piriasaa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dkbqlqbz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2xibgjrvr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cawzuwip.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pjqeldai.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xoevmfjd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ozdsiusk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gwzhplxv.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aluxyrml.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2wgnvtjii.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ewhcddyj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2zxofzevx.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qdjwzzvg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2azerbhef.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2alyeeofc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oygwgdvv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xyvedayt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nidxoeqy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2gxqnmljq.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ecuqqgmr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2wtqzvdfx.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfskrx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xjolvspl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2manqvhgu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqwdslbu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2tshceglj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2utbshfrd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ltcpxyjf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xhbfnpuo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzvsqx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jthvlxve.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ttisxdgf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vmeeywss.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nnixqtbo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2exvyllry.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mpfokewm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2fxhhfvzt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2onbztsrn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2sfrmywaa.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2typjxqag.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qrpusduc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2seqockss.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wmxdhadh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xmspilyi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2weyeaorf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ojeqerqt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2jpbwxaks.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ogxoxarz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2tticnxgm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2gsyodjzh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vzoqeife.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2ibidhwqg.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2uochgtpu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vyoegldk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2jjvbtzvj.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2slowtqsv.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ucdirhbu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2oosixslu.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nngovonf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2skaisrfl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ddswfkmk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lpvgjvlo.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fnawfhdm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tawoweme.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zofdofrb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2hrfbjcep.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2rvnzijyr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2oisqrldq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2vevpjmgf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkembvyp.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2zfsxlfla.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2uavcyned.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2hlazzprz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2knmzncrq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hlnlyiog.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2orlnevgo.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2pevzlhur.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2shdsqtzo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2rtwbztcl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2vuwitkyb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2dcywghpp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2sbvopzqg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmktxurc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2aebhaszn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bpocqqxu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2cmootbcw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qcubdpkf.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bjcjouyo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hvddqzfy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jokngtkl.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ohnkhxaa.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dbmpzcvc.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mvwxpkbh.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bjbgxyhu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zsxpcoki.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldlakqtc.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ynplspau.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lbxlkgxh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2jbdehjiy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2xzmriozm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2dyonsxtj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dthqpovv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2dztlulhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2brcevtip.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2kawsbvtn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2qhyvycmr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aynlrgey.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ueeehaou.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2xxbunxyz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hgmnsnzg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2poraexnb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rfogchtc.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2tzniphte.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fgphjksk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hmkdqzbk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fzyhvmuw.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2dhllizsw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dwuqtaul.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2inkexztf.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2emssrsxc.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mjoyqlci.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2wjmhbclq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2qjkxybes.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2eghmuwmq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xjiraxcs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kuquxnmc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qmgqgawc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2mjzxbjke.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pwxlsqlo.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dmxsztul.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2pknlrgny.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2oqbgfdfv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ablsajjw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cgbslldz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2emgzkbyr.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2eihfncmp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2exmifcdf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kvqoomcl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jtzkxlmr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cwtetpil.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xjmidvrq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2beomaqlo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2xelqqzfa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tjwjfebs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lnkiretz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2sbyeqyas.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2rfhoayvd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xxfmgkkk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uatogykz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2giictrnd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qnxqyvkb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mdtmhzte.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2goosuzsu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2wjfoauke.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2rlfqrkha.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdcglfd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kwxpbaly.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ughrhlai.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2akwkgnps.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujppoyyr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jmghddnp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qialefnk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2sewitldm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iizhkovr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zoovymdx.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cpxdetzd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2trwuirmx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sbqvusqm.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ffxbbpav.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2buvlbjrx.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xgzfmxrr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zulasmwo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eizkjdud.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fuupeexe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qhnphxja.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2iiswlmsx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cfunwdfd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ijldifzj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2rpycsaat.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ywfjonbw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nrnnljrt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2edhpjbbn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xflcczym.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2azvfipaz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2giqdooih.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rrnvcjss.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hhopwmrj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qhljpscn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lcmloios.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2abjfgfux.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kgfguaqj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vzrmqrug.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2amkbzpyz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nikhulqy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtwvtl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2ynlzqzjo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2glhvtgsx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tlerehpw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rezttala.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tingtvve.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2jgqaqtxa.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hljzsggh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ubhlhdwa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aebnicph.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2iqmmftpt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ketyysly.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hshwxlcr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lqoqwgxy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nguygejd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lxjtagdd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wvihzkvn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2qiwdmlay.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tptrzrhp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qjnsidda.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2csjnnktp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ikcjpcuw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2xjxxmiye.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2dqrlvqck.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2pmrdelta.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ltnfwgsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkyaaslg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2okjhyzzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuqjqxbd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2rqnkmawp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2useqwaex.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hormqmbi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hizwkgce.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2usvvckvu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qxfmedky.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ecdrqyek.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rbkfbqal.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2urkizcck.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ivzrpgqn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kqimkcur.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jktmvnyd.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ujnulzlo.html


<!-- 参考信息 -->