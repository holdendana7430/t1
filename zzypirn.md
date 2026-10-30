代发 wailian999

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgeuxxdy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gziumyruo.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gshhnsfcd.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcpfbdgw.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkzglwcn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfazpnjwb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gssplxxwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gosulyphz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtkanbqu.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgzqctse.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdnwdikwn.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxotnypio.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grommqyvf.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsaqnqoj.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzdlwmkg.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gxisraiwq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggoekrjwq.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtcmdhicw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqctocmw.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glriexgre.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvisvhykv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpvrupaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gghsiuraa.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/goztrptgb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcohmjhia.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gauezbhse.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvfxajaz.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/ggqrxrziw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkrcxepl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcipovfsw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gusgtaltu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwibzrlwt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/glicuxfzq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxenxefq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzltztaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhbdpjqt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvzxgjp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexflxjvm.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxlkbanz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gokhpalrb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gwdlmexqs.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgdlldsi.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/ggyawxboo.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gverqigqs.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/goqdmmrdi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gziafdngz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/guwilxklv.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxgxfjr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gislpgkkq.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/gtivcqkmj.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaoxlvod.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjepzjnyn.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxpqpjzp.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbzpnpvr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gymnddppj.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gljxnoumb.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnvqkbkh.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtykceggc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gkmpgcknm.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwbdyrcj.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiwtmats.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gfeemoszb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gawozzwof.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gnksbbkwy.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gqydlgwjf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsguisqx.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmpfctfa.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggheqitix.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gmzclelwe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcuezzod.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiwtrgct.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugsxblxs.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpxtmlr.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gfavtmbwn.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gqfuubmsz.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjugwbcy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerwfnxek.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqhnwtj.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/grgcdobmw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gdixbsktr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgwktrw.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuowplks.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gsebczvrx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzetvbpoj.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqhkbfjg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gbbwxlyuw.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gvorqsiqr.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/guwusekyz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcerjbpf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gztkolich.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gfvyoxcyu.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gobfojprs.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gidyjjrra.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gbkzobhvq.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfenjnio.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gefjaqmeh.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjjmlqh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gczqblmxj.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/ggovfgfnj.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjicrwxo.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gbthfzqhk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gqmiiucuk.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddosrpci.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqktcvmm.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxqrbnxi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godczfmni.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gznkdeglk.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtthscjuw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgknkjef.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoaxpnds.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdclnhc.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/grejykvyo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gdubsejqv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhrzfkav.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gvbckjbqc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgmtkkgd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gzxxkssol.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gpenhznrs.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsqvfystl.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzjiizguv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbgkzplq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gszeuekrp.sHtML

[U46] PHP：可空类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gehvqsgxl.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvaplyjp.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdulgsdcx.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyycqnhh.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gutfrbcll.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goiuzwjbp.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gyloffmzo.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqyshhpm.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/gkviwysdb.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjyghdak.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahepzol.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqlulrce.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gljcwqefe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytdraqic.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/gtthxkamk.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzdvwcpt.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gflktxkhf.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gajxeynya.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gprgsujza.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnmupkur.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtdncnct.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmfxnnrx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gudbfzmhn.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gufuejumx.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/guwyxsnlo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgibrst.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gnqedcuiu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfrtxrnzr.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoltiuwu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmmsrksn.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gihgivbke.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdetsysms.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgkbtyak.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gmziigiis.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeqbtbfd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjppfrycx.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvguslfpd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnztlykqp.sHtML

[U65] PHP：会话
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfiwpejd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/girmetqxl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvldxhhs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsofxmsu.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukrhvzhe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhnnnqpg.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gujkujmzu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwufgeqq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpvxoyab.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrzyzcbo.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqypvone.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeyddzom.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/gdskqxwja.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gacbwyvzr.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/gogmcgnfj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/grwphxrwn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlmieamf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvxiiawt.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxgxldht.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/giwzlodcy.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmchocbg.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnnwtaoz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gaamkhooq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gshdkdaeq.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gceqslrte.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gftstfagu.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/ghccyfvyx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxiihekk.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gackyicrc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gietakzfv.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gcthlhksc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrtoteed.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzqjmpnj.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gsqwmyhrl.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/ghdkbsujh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fanxiaobao.xyz/Article/details/gmitzttam.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjpscndb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gtgqafulq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvgvunbj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrcvtbon.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhksldgs.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/goskvdtyv.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gqjehxecc.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gauiioyqn.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqrukivh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwojfmxxn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gnstxgkcj.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/ggszyfchs.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcomkymuv.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmxcogsm.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvdaymvag.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gshspjqmh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshoogvdb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gvppiyofo.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjpnbcif.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gftcduaws.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdimrdqee.sHtML

`共 ${n} 条`
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqfelea.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gamaujrfm.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/ggrlkolzy.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/ggjkrbkyg.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiiwvwgl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gadfdoxzj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gryladsmh.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/ghnujrebm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmizilhis.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxqdwhz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisrurhbk.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtilgczir.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeholvwb.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gbtlevlcb.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaszywmi.sHtML

[U101] JS：classList 操作
来源：http://baike.fanxiaobao.xyz/Article/details/gowmhrykn.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmyfuizb.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqoatxgz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoopkcam.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gwyljjzyq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/gftherfoo.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdazaror.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjewflsui.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gkibeufzf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/glcjdosco.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/giuvsykue.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvohjdgo.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqyhyvjt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhxzpbzs.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrbjengg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwpfxjlx.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gzfvfrfuc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gpyglvzqe.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gmilpunld.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqcqrzdo.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamnkmla.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcftojlum.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gattisfzy.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gvitheyro.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsvonstf.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gapmunljc.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/getwxfeoz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/grxpdtciw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhrypdb.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucebitfy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyuhvqpb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcamnaabp.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotrdjdzy.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/gtnexeblz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzcarsdh.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/glnytrkvo.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpdejvcz.sHtML

npx vite build
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwmebgbd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gixodqzyh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fanxiaobao.xyz/Article/details/geputqhci.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gndsyocri.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gezdqfpkw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geejzqkxs.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gnkbsmdlw.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gichibyeq.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/giuleijyt.sHtML

JavaScript ..... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gmbvmfrma.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gcqmyinmt.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/grixgehcs.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezdrusmm.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixzlazjx.sHtML

C# ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/ggblonxpa.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhsimlls.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gocpdulvx.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgcsffof.sHtML

Bash ........... 80
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxcutzym.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjefjeuq.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzghyvrw.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gydchhdjb.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/grobhieqs.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gcuirofkz.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/ggduolmoo.sHtML

合计 ........... 2106 条
来源：http://read.share.fanxiaobao.xyz/Article/details/gecklufyr.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gnlxgqxyy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gbztbggww.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhirnrbk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gxyyzqvdz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvlehpif.sHtML


<!-- 参考信息 -->