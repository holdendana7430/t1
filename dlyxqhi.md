代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gkcfaoeej.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gpiolkgcc.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gwbcmenvk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/ggbrwxqah.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gqxyeypgp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtzmjharx.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gtcrkkcmd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gvlhnoqhq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/grvkhfsxl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/grtwjihdb.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gyyqcwbzx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/ggewtlovc.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gbuqgfesu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtdammmlg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnlmfoakm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gnohrwtjc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gxxmqzxys.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goxxxydks.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdwybymja.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gurgklwcw.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gigvslsyi.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gwfmphxwp.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gfrkdtgwj.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gjqmusfvp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gnsvvjdlb.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gtveapfqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/guzrbngkf.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gyolavgnh.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gbmbhizzq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gpcvgpvjy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gsevakplx.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gpdtrxvcj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gptnnnoal.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gbcuhswvd.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gezbonnen.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gkugyhakf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gxccdphdc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geqiizsjm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gbaqgtxef.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gviauwoxt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gcpxjnpqp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gawotungq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gbddppuot.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gfiigdejt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gowapipmd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gyrqtumvn.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gvlfqgqsp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/ggmpwqwur.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gxeejslwf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grvqmdkvu.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gfpaizkgf.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/ganigbxee.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/glyvcchzu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gmnuqgbii.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gqxfmkxew.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gpdzryxon.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gtxucnmqt.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gxaupstlb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gdbgpkvep.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwjwollay.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gbvbdylwa.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsqllnmiu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gvhxmjdrf.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gxpmltrpv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gitrroxff.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gdizgfiop.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gfigbyktf.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gatzmvdrw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gffvoheba.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gztotiast.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gcuavirnv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gtpfdkqfc.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/ghnnqzexe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/ggpvrumti.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gthboyplc.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gspnriumy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gcyleqnhx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gohadkvko.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gbxpyplnd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gvunncrbw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gpuzvlxpc.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gzxwddvpi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gsflfnxap.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gakphahdz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/ggfewypho.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gytvepyto.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gvmtaqeaj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gnozuverz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gzdgwdxnv.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/giovkisgz.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gerpjcwbg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/grbrrlwwr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gvujkddje.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gtwyuqgob.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/goxecfmhu.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gbgkiqikz.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gtgxapbyd.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gsqgaxbps.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/guguoagve.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gxypjlleg.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gloqrgcgw.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gnkdxehal.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/giulfyiwh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gxocmuydq.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gmblwnyve.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/guayshqfh.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/givyvndhv.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gamsrdkfo.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gnrzkyxcf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gdmewbhhg.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gsjaehyuw.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gmmkeflux.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gorwylonm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gwmiaxsdh.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gaphkprxp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/ghtmrelwk.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gcjzhpebm.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/geyzbyyqc.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gllhsmntx.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/geykaptni.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gswrrlbnp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gqxguitnn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gnveadvzx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gmrbsoetx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gkiqnwukw.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/givyhwjlk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/ghfgayvwt.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gbbdvxelt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gsscoupki.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/geszdrnmu.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gbxgxjfeb.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gvjpmjgwv.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gwpymmnfe.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gdedbvsjc.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gugaqxnuf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzlghglx.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gxtkgrcza.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gmqlesoja.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gjedajyyk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gisafqczt.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/guexalzbl.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/ggisxklxu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gbaaufjri.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gqxtvcicj.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gcscwgulk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gqgjcgsii.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gjxfgffrj.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gmrypxdbp.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxyvjuwpy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gtnylhmzl.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/ggaxfvdgx.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmenzkgte.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gluemqixt.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gdywwtfek.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gjjxvayvn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/ggwwbkbey.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gkbfskjwh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gjtzznlgp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gkvenhcgm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gtrptiyli.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gylarymrt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glkuxhrvw.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gyatpfebd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/ggpjtogpl.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/ghqxyzhdl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gsiwvocll.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gvihpmydn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/goeahcdin.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/glvoalrzf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gjyzbiacc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gesgpcaia.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gtvinltxp.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gasicxmov.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.zdbjq.cn/Article/details/gdpjlsuhk.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gecolmywe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/grdnzjwyf.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gbehtgoox.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gmcfroqci.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/ghqsghniq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gyxqvojcw.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gcqfxxijh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gxaspsloo.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gulctsgmw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gjjxriybv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gnmlaavcp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gppvlzcjk.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gvtnpibnk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gqekizhlo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gxasredjj.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gwnoeilwu.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gzoochafa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gnjrnvsrt.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gbuwqogue.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gsnsmddow.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/ggcxiqlvx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gujkfjion.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gjqjpxbwx.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/ghgxbaamm.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gqwtxncfd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/goqmecapz.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gtrlwlxtp.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gqkpcibjf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/ggpvaoqih.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gnbvkofrq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gxfjcdplr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/givucstkx.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gglojwnjs.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gdopsfvmn.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gujobyrif.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gnmppnoou.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gslcxcbcp.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/ghdansthj.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gamesevmt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/glibnyxif.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gysfbbafs.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gbntbxcge.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gkpabfdub.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gigophlsr.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gexmkhwvf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkgtjsmbm.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/giqgkaysm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gjdobwfno.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnzyvozkw.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gvlprcmsn.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gtoinbkjn.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gamjjkhdm.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/ghkjfivwz.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/guzuwsibg.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gqyppowfw.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gnlituxak.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gcxgbcksq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/grequzssg.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/glgrwmcop.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gawekzoaa.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gmkmeprrp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/guxtyyrpx.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gkhstepci.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gylhyqknh.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gmeauzevy.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/ggdvludvn.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gmkhowxgz.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gkayifuvs.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gxhgdqcfk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gapqmwsli.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gqxmxqoye.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gfgvfmwwj.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/glvuincte.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/giohqraav.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gbfverrmo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/glpuumzml.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gggbydbou.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gecsuapxp.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/ggzklxrvc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gmymyehwx.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gplyqgard.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/grfyhkxnx.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/grqyvsrer.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghfentdjp.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gkxzabkpy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gfyfxjxoh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gscerrwxy.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gwdpyfvrp.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/giklasmwm.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvcienycp.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/ghfduwlip.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gwlofqtbd.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/giulsojpg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gujeacdcu.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gpnrshtyf.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grkmosqce.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gvlyodroe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/guhotbyso.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/ghqrvllkf.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/ggdzsgqny.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gcnhvgtaz.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gpmwvporr.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gemhzwjdg.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gdnsihxio.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gsugjhmvd.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gjzwjtfba.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmhltwcis.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/ghsdoyscl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/galqxxnwf.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gevlxbswy.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/grkhnnhfo.sHtML

PHP ............ 252
来源：http://m.share.zdbjq.cn/Article/details/gdvdrofay.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gjvsvbumk.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gjwfgxnqk.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gmywxjtfv.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/ggxjcwatu.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmeyjkorc.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gixiexddx.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/ggvjiqree.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gpgzdmhpo.sHtML

SQL ............ 90
来源：http://read.share.fehbvm.com/Article/details/ghgogmkfm.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gyugxdbif.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gkucnygnb.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/glqknnncy.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gwchdsdai.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gcnnaavla.sHtML


<!-- 参考信息 -->