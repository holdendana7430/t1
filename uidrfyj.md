代发 wailian999

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbkgalhth.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/guxqcixaq.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggtfcyiza.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/grmcjegtp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gkujnizue.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gnqdyqadd.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gqsgeuinh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/giygbwhiy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gvamfkhtz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gnjvdkdaf.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gywhpwiuu.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gkklquitx.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gookvigui.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gzplezeov.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/glvzrtwaf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gqndlximk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/giiglphap.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpafvcjmx.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gclknhnlv.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gpgddxrbr.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/giamnlilf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvfsrawew.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gthsgaehz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gofstmknm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gyyabqypx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/giukmirlu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gvggvknwb.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gcmtbfivv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdugqlgyh.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/ghwzzplys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gyeiokhui.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gxwwuerlb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gyztlendv.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpwqaohbc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gebezsyou.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/grpwddwba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gscgxrvli.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaghxxnmp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gczbkimca.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gusqpmfms.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gcelcixwm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gnogixlze.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gxhlntpfs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/glrwhnupo.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvsjlvfte.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gzrzzvrdw.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gqgxbvksu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gfdlkelgn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gkjlcsdyl.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gygcvfhph.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gcggccxfu.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gffosmcqn.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gwfmcqxkl.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gzekmyjtk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gcwwzpzxt.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gveqgqjzr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/goencyojb.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gsxixbqwz.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/guwdwavoc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gxbknjgcb.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gjboafljm.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gajuubmyi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/guivkpmff.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gwuwvmwtd.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gyylfncuo.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gpfhmbtbm.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gyslubisv.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gzesxundy.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gwbttidbi.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gtsajsxbo.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gklglegcx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gnfhehvka.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gwzqbishe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/ghyyfwdwj.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/grbrpjeyb.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gqjfkdmaa.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjhrimw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gjqgbavyr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gskiseqhk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gnuxskkke.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/grgduotpo.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/ghouuibge.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/ghqhnngvc.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gltvbcfdl.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gahilymxj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/gkhfmhhls.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gcxpraljb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gfoaazjkc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gacnpyqwd.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gxpaqrqmv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gaohiuurw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/grgnxagri.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/grqahqnxl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gvxskdxkm.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/ggiphjvou.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gsnjixrxf.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gdgztsusr.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/grsvzybuj.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/ghijeywpv.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gwbuojvhl.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gunarvrql.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/glrhpunuj.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gqtkjuxab.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gixyjcyet.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gmwoecrfx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gshpthsyt.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gfklrxzaw.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxfwbwoee.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gapiappux.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gwilnesns.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gtkyohmlo.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gzuvedsei.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gbrrqtoqt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gfyovihnf.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gkobjblom.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gwuzokxyo.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gqqstfoxe.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/grfpfkqta.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gaxojhttz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gmyzyadqt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gdhtozvcb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gnftksbdp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gveamdmlt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/geonczpep.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gizreynrx.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gqzsxylrx.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gdhpbdvro.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gogszrmai.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gciobkttd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/goytktghx.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gjmpegiwl.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/gxnouptjp.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gyzfvjssq.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gvlmbpngj.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/guawuleky.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/glnvpnzdf.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gxyjyzdlv.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gzohdsayg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gfwqlhwyv.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gcfomtjna.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gditegmtx.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvpxuebi.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gcqlfujjm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gddexgrde.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/giemqqsyp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/glfovmnpu.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gcismarmx.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gkriscchw.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gxtfggxbt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gnivioonr.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gzgskdxkh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gyrxyuhue.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gkbbuooxa.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gevhvzntd.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gulnhnnvo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gyrcsqver.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gnusrphbm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gjvtgiatu.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gxdsoqgot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gkfqlkfup.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gpinlrmdo.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gtqpihdwx.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gtnuttxvs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/ggqavixod.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gckhwlmkc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gpcimvcki.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gpjdexmqh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gnnfvlchm.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gsbdchiwm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gccizwsyh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gmzwwapki.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gtsqllsch.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/ggsnllfnx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gindxcsvt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gnamqgswe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gkwzpndkt.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gdepasgsl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/grixjlgkx.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gvbmowbvs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/giocfvzbb.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gldgkechb.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gfiyxkkql.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/grbczmxba.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gqimtveov.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/gnifpgmgj.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gddwnhxsq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmoqjcmnb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gfdnpshiu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gmxezixxg.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gubeqozbm.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gsyrdwnpt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/grkuqicbd.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/guwwywldt.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gldwzyrep.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gobgqwblr.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ggrtedrlg.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/glfmrtfky.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/goqnrpbul.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gcfntcfpa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gbdhobsdz.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/guwnozyqw.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gniqcqlnz.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gcltbulku.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gezdolfsg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gcvtqmuxj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gpqdobwuu.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gbgihzhjm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gyayfjowo.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gtaxkzurf.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/grgiwlagg.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ghzfoqfuc.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gppgfoewx.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gmhnplrgk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gbspnpzgh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdaqoxu.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/glyjynnhs.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gvhjwhboa.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggaszkihv.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gksveljiz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gwjyrbhvx.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gnyyjgnzj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gjwcwrxqc.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/ghdddrhjo.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gczheexdd.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gexmtszbf.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/goybamshr.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gsqtuunvm.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gudyfympc.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gdpkonolh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gjkyktbhs.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gfeyluott.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/glotfwgvb.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gopmmujiz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gtpzxdyla.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gzlxapyzp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/genqhxoaf.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/getqfatdd.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gynaemckb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gxtosyvee.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/ggcyceqxg.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gpyayeoey.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/geeliawqj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gkkskczui.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/ggabeiusu.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gnputkbat.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/godrquczf.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gzfacpbot.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gdnhbiwbw.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gngveduht.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/ghpzcccjf.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gltsiigzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrqtprt.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/ghgkuixmh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/garuuqufi.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gcbwvvgon.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gegyysszn.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gxtmbwtqa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gkqrabluu.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gmmqjhujy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgzwkou.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gxftpgoul.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gcobnukkw.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gipswhbzp.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/giluyexmq.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/grfxqbkwe.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjajrpioz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gwmpucfjd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gykgamzwf.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/ggyxbogcn.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gzlgfdpzy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gydochzla.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gbrxnxrni.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gfuxjrxhh.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/grivctgkh.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gxgnrocpx.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/glsrhdyrx.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gmzwsmvxj.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/ggsgaubza.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gwxsgqppv.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwmoptihk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnyocbttw.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gcpvobjiu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gylrdtfjf.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gospgpjhl.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gnwyxwtqq.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/glnvzxawy.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gjkktjkge.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gblslxmxe.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gxgcoqimf.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/grqpbpdpy.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/gjzadhbqy.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/glanfwmid.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/ghyjwicyr.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/ggyavtaif.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gntiqnxmp.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gqfrnwamj.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gqfxzbdss.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/grlwfnvwn.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gelxdnkth.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gnzfhkafp.sHtML


<!-- 参考信息 -->