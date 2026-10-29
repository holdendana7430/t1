代发 wailian999

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/guzmmtmvn.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gqvguaksd.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gplkqjztu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpnmaowwb.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvypzeejy.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gnddvicsn.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gxmmmwmqq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gxckcvmmt.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gignrwqdc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gbzfmwtfr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gmgfdidph.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gvgxldhwe.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gmwdssete.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gkkwrrzwr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gbavfnazw.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gqphpxsub.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gowvqvgpo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gsdwrhfvu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gxfwvhawj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gglauhlub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gcirsarmd.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gerfkmgkn.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbqkzopno.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gvtpnmlkp.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gngjwylcd.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/goxkosggh.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gkizmwwnp.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gnngjhydj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gdjnyaaik.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/govtmrdxj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/ghvwhxcmv.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gimcvnnhl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gqhyuqegg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gihwvinwo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gvxtjkqun.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gswufbete.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gvwpboxab.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gqohqfddm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gqfuhgecx.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gdazpvvfn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gephcnoyo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzpszmxyi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gluktappf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqnxzsmuu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/ggyhhyxcj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/glfaccfyg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gwzcaklgw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtnmelmdw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gjodqciqp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gyoyubyzx.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gxqtnyyfl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gtmqktngt.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/getysoauc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gtaopdnbw.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gnspxbdax.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gypyqrhim.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gtnyhdqdb.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gxvxxpseb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gaqgrfkxv.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gheohdglu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gxujqgngz.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gzljfwysa.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gayeulgvk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/goxztfkyg.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwxjxredr.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gzzyxrhmw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ghcrebpvl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gsbqdmzlx.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gjntqeoqy.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gfxwsnrdn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gcvifysow.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gngfqfpdq.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gxezttugb.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/ghanbqhby.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/genhvagof.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgwfggwp.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gmjgivahb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gqpbhlhcv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gcvesrxwt.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gdsjcdudv.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gjospofxe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gpvzndayf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gbpkxmkyw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gdxutaekc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/glmmuoifm.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gheguazez.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gbrueejfw.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gngfeppjt.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/giubqxeci.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gozfuazom.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gcgoucbma.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gwunkfadl.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gzeznagyg.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gvukkfrze.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/ghrrqcukg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/ghjehgfmo.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gutthmmgo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gcryanbfj.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gqgdryvdp.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gkchjpzbu.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gmrtsozvh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gjqjwivue.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gxiltpnpn.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gguebvhcl.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gohazlvju.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gghfgvter.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gmxcjnado.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/ghervhuso.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gtltpkvif.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gcujjfcob.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/glutsoabi.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gdhqrutzu.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gfkexwnta.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gqgkbkvqw.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gbhurmdvl.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/graoanuts.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdwdphn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gldjyftsi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gvrlkfroz.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gzkblrvvp.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/gjxpbyyjf.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gmqhonbzm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbpsagp.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gwzjvrvpg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/giwpvhwjs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gspazfuqk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gpmpcjakl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/ghuhdgfim.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gidpmqyhn.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gmipaqtln.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gqlkemups.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gxbhsinzs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/goztbjzxa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gysiatvyf.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/glapswqtx.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwigxch.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gwooghpig.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gzftlmjfu.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gubidyxxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/grbvnwnxr.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gfwicfoth.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gkrwqljsd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/goqjirppm.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmipazfaa.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gndlxmmtr.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gjsdlvnuf.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ggwxrgclk.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gmqvzoozw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gxrwmordh.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gjudbrldi.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gtbbyixkw.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gxzsocpef.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gnkzbjqls.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/ghoyjjthf.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gsfjmnxut.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gnmkbblaj.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpmybfjsa.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/glqzpbyuf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gzpxkavrq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/grpamxfrx.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gypmhtgmc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ggikwftfq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gxhrfwsaa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gfzhrcoto.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/glwuhymlb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gpnlnmvmq.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gkrjnfmzf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gfseknijs.sHtML

[U63] PHP：文件读写
来源：http://read.share.zdbjq.cn/Article/details/gnzsxruwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gzevbgrqr.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gpfytrxzp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gkoteegjx.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gwasudzgv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gtrsuvjbk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gjxzlkycp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gmkqcmwjm.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gnmpndhal.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gyijcpjcs.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gwkqwbycz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/glhmhbecc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gotjcukwl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gwiejkbtv.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gtrryhfle.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gsnsoiwsz.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/grjndofrd.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gtxzwlokt.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gzttcsuge.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gvlwpucoo.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gkxlvdmez.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gwscckoqv.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gbannrmeq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gqssbbumg.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gotlunicw.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/goqjczgvk.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxmynjp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gfntwbqjk.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gohdjajlo.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gyhrplqge.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gbrqdgcyj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gwxwwnter.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gqbkgurux.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjdazjt.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gqssfpwub.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gvimphdno.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gpshvhpjo.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gbhstglte.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gnnxcixxn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gduvgzrjq.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gazwclgwt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gbowjkvem.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gwmtcfqki.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gukqqtfjq.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gwutohkeu.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/grmhscifx.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gyzthdilt.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/griwvtosr.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gkgleafrh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gjpwxoalj.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/geikkhjdl.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gydtlhkua.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gztdnybqb.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkfmcounv.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gmtvrpkrf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjcigphla.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gmklktedt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gewfithud.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gijmadjio.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gxezjyzsl.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/ggqxwurcr.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gaqbkfpnr.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gibmxdedm.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gwydvdyki.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gvnhlawlx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/glbxlhrmw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gmpiylexj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdmrqqudw.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gkdupssnf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gctmjhyeo.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsrnfqbiu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gtfqplxhe.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gxcklumzp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gmgzmpcpj.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gbmcmhqlq.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/ganpzsuof.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gkxpeorof.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gqxqnqjgu.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/ggeqqsoba.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gljynnxoa.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gtxkairsc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gqqffajdt.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gnmmbhfwj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gyjpdtzpd.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gapfomblq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/guawekbtl.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gceblglxq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/guigclymb.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ggytubvvi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gnpdrtroj.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/ggrxoprap.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gtdegvnwc.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gozndodbx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/glezblhqp.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gkmzkapga.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gniimfyot.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gubugrcla.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gtusaydmb.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/goyeciudg.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gaocdtkdl.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/glyhwrkch.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gokolwysn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/geziufdfw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gguuxckie.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gamtmaksc.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/grabkasrh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/grxuosnyl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gjmxrdbbq.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gkcrguyls.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gjdexjgvm.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gyurfrmdg.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/ghpztozdh.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gdkmisbkd.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gldmkenyw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gnsmebgho.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/guyemmoti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grwvyyfde.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbnuiaw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdrpcvkqx.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gszwylwiq.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gulnpfhpw.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gqthcuwzw.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gadwbfhuu.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gkxmqabcp.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gnnaoydti.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/ghcabesaa.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gyxnpmgiw.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gcdqfotnu.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gedekhmrn.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gsqqjwycl.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gyqahdvfc.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gzogcwuww.sHtML


<!-- 参考信息 -->