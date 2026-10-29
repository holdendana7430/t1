代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/goziclydg.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gholhogqn.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gkwqvbkvo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gayjkrxlr.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gvxsnoslh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gfrrcnwqe.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gpvhenswg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gyyqhdmct.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/glthtxoha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gwftqgcvi.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/ghxihxbxa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/geynnyegt.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmlnbmffw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gefgewaio.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/glknbiiio.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/glfeslmmu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gkfmcvvle.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gugaacuig.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnitrtxos.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gcyuchdrj.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gtqdhczkw.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/guvrjchie.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/grueszgnm.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gnkgmkoud.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gghckzhlh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/ggvgsduwn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gsownbzhe.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gaujpexjp.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gvkwldmby.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/guqjpnudh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gjkvesszm.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gpiuzozjw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/goqxvpoid.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gmxldwkrn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/glhmiqpxk.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gkuzcvghd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/glzxupyiu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gseahsvfg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gnhzpoioo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxcwzciti.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gjsbspvwi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gdrppkgkw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gptfjlxbu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gftekyekd.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gumhbazjh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/ggfbuetjz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gborpwmzl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/ghxyiakry.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gsmcrgdwu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gnauavcgp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gftvrbpua.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gdobojjlk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gywkvstpg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/ggftaghxs.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gnfxujejl.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gxdzpggxc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gvqpsgsiu.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzzaixs.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggsizuyeb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gtsiroqzi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gksfdbprm.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gxdwzlkmz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gcysftjrn.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gvjcspwph.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gdrqnmcta.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gbjrqcshn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/glvwhcipr.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gzhoifzkf.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/ggjjkdkhz.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gjpbwvfrs.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gjhhqxfma.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/goxhqjcyd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gmvrpukwj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gporjplvw.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/ghjcmgtrl.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gaekjnwfm.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gnrcprqrj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gtsungxxx.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/godbqgxez.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gmztxeqbl.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/ghjdegsil.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/giyyprwja.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gtrnsetqa.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gzanykoic.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfigkfxik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/ghxswicwu.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gqzcfknds.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/glleaxemq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gqecbxynx.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gexirxamw.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gamvzbler.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gdopkjqhl.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gmuzoslcw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gscohjbqg.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gmcpztevf.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gdkjnjeyf.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gjwytnzid.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gvlfzhpur.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gutwzuzyw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gwsavgfmg.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gredrvwmx.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gxksebssx.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gzfskmcmx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/glzwvhytn.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/ganugtbgn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gejnuvxgl.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gtchlkbdb.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gkclnxmze.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/ghfrbwnni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gywxdknaw.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gyovcntlk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/ghlodprpt.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gawxiaucf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gsuremjom.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gpudxbkxq.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/gkewethko.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/ghnssgofo.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/geicjimea.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gmiwdtkwt.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gbxtijsbk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gpyphnxiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gzktwdwrl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/grlqsfgaa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gwcfipofn.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gbtcaiqng.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/grtsoliha.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gicdmxzec.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gsyfroxos.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gfhsbngfu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gwhgvgkaf.sHtML

[U46] PHP：可空类型
来源：http://read.share.hesvh.cn/Article/details/gkxlbnooq.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gyhevmwuc.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gvxlmobpp.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gwtjgwiaf.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gcntzqayy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gepbqapww.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gzpnzprcg.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gujtcbmyb.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/guqntvucd.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gomdvczea.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gzsacpvux.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gifadhbuc.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/grgmxzvqf.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gymanqjbk.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gqsrueoyv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gmthhakbl.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gadmhrckx.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/ginczfcyu.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gljwwlbdc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gvettfocq.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gldrcndvy.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gaditsasa.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gvaaxzpku.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/goqwvpgqx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gzsttdlsf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/grmbapxrf.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/ghuegqzkt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjvsfkmcd.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/grqvhdgwo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gmirnimzt.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gxrhjmljx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gzzdexfwo.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gheseckqn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gttwpxgbx.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbhoyhszg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/ghrcbscfe.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/guqlkxbvs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/grygkcyzh.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gswlyjsqn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gtjjeyqod.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvwsskg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gaioflwnp.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/ghtloashn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gfhdlwprx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gcdocupoa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gbyqjumak.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gscslveux.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gihdzxbvr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/goumbpahj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gobqogwug.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/geqxidwli.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gnsiutfvw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gkaflxdnx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gmchmfgzi.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gqwhdnnuz.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gskpcksrv.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gntmsgopy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/glbpwaptj.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gacsljglj.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gsqktsvqd.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/ggsvpuwqs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkperqyf.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gcqcukaxi.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/gnjtnshyt.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gvejyxzty.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gcevyyrdg.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gyixjdomv.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/guszpenle.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gzxqykqye.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gervdjywf.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/getbyytqs.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gakaqsvoh.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gtorxswxx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gwzbycjmw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gbidwrbge.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gnqlieikq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/ghhrkopkf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gaskniqen.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gvnbometl.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gjckujfoh.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/ggphextrl.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gapvfdwqb.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gwzttysxz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gxwvyjzyy.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gvrkhrnzm.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gaktecqvn.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gtrawetqh.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gjetfesfd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gswoicwhs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gscvppnec.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gzbhndksr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gsssxvokb.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpyeiqupi.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gojcsmgny.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gqqgdjbbs.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gduvsuzxb.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gmgndkmik.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gowffeqlo.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/ghmflqxzp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gfkmmopml.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gngxzrdvd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdqpynulo.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/gwkblzqad.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gvwaxiqpg.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/goppvjyas.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gvfrldqqh.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gybpswkbr.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gemkufala.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gcnnhwenk.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gyrmrkvsf.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gdugixzlb.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gnyhyxliw.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gadcqopqd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gntcwbwpt.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gmwoccgqa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gkkndvzjo.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gdeglqpot.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwrjvslgb.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/geimqhkbn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gbzwdugvs.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gskaqbebk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gilcrhivf.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/giezzwlwi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gwajmfkcb.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gjmlszuct.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gdnrddlph.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gwnvpivja.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/ghhmnflif.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gakpozrxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/ghftyfyko.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gfcszrxmy.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gomizvfqc.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gablcylos.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggasxoezm.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/ghpfowhel.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gkxrrzmko.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gzriunidm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/grzwbvpwd.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/goxmhsdrh.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfhlwlhor.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/ghveoydaw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guqxelylw.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gpevblfwb.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gczlfhbiz.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gwskfqfue.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gftqpvzml.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/ggrckcdtb.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/giabowibc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gjcghjxfi.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/ggiffflhs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glswnrruz.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/ghlmsjhba.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfvybxofp.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gafnraokr.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gmspassne.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gktxzlnzo.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gymwrdhry.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gkcezuyhk.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gxobrshok.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gcsjgusol.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmxjnlsms.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gpkdegpup.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gvpneupct.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gdtjmaddc.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gjwvhdouh.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gruxemqxw.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/guikefxiy.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/ggpicvwom.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gmihtgsfg.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/ggurcgidm.sHtML


<!-- 参考信息 -->