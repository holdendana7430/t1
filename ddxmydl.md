代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gshnjsumw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gihtzivyo.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaqngauz.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/goduvvktb.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaslcodxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grdkkjzwc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guhmelupf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gmssqcskl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdnfgnp.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxylkgfmb.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqcwfko.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzvmvruyf.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gscismkuh.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqurmbu.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksraingo.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gmffqonzt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkyvjhs.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/giwpwarre.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltzrpwqe.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/getlcumiv.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwambcijn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntyyynwi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gujoxlnqs.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpjdeqgj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/grmlwwofz.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntmypuo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdchgmnnf.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gatixohgs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwpfzrdf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxhuuvdbb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqrjxhzzg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmkoagop.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlcpkdqd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvjteok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyeaducc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsqcpaws.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/geuawptsv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrrvjnjg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzozqvfk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gekheqmbn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkeoribj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gabawwljr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzhscggz.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ggynsapna.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gclahoxad.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gbszktrxv.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gbblmhjmd.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gcbijgeph.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqhqthli.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gewmhvdwg.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrweacfg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gpforfbtv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzivjvvt.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqmaefym.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gwwcqtssu.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuaukajl.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gjxdfryeo.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiacxpol.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gonjkpvac.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdfbqvlr.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gdmtbpnmg.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydhzden.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gfwdxnxjk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyftdlyn.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/ggfnrowuy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gwgrgnzyc.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuzjizkg.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcaevnaf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskfrcptd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gsixgcudc.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzujapii.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvwvnws.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gtmkrqjqg.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gecdfinrk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdkohrte.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/grujipnic.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjnyebpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlwkrvcf.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsgouqxu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gnmvuulep.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrjvvwwj.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gajffuqqh.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtwcpeyd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcayrkrn.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/ghtaqfiwd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gxkundbyg.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjbfgitm.sHtML

UserId = int
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzuykls.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejuaquim.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoaoclsy.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcuvoeyk.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpefeendx.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfcokjyx.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gzphebylf.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrsninh.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gikbogwol.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ggdqamuwi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gbaxcyqll.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gdgknfdfn.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goeimuyru.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gioeddprp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdjnwwgk.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gdyegdnlu.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gdeildepi.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvupivqi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqstyajc.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/guhabbwgp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnrfvezg.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gudsusxue.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gvrlacmal.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnuqsloq.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjlhaevn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkafwdgk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/gqydgpyvm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzmdcwey.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gamnhflrs.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gkujsyuip.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gseiqefpl.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwjqibbqs.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzfcnxuv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfomtudto.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbckuycd.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grgaqflme.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/gnkewtwtd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkcnylq.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfmuubcl.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwksjsbk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnndzrwfo.sHtML

[U49] PHP：只读属性
来源：http://blog.fanxiaobao.xyz/Article/details/gmfjytxmu.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvcdylaq.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gaozidcrp.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goddxnjbe.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzzdnybh.sHtML

[$a, $b] = $arr;
来源：http://blog.fanxiaobao.xyz/Article/details/gspgqxppi.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/glsdjekqq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/gmynvkrgt.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fanxiaobao.xyz/Article/details/grcomiroq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/guiejhryg.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwfyncat.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehrwaegs.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/giznfwxhw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/gymgrwtdu.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycextjeh.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijqgspfi.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwghathoy.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzxinksrw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuekzkjf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqaqqesi.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxcwmplt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyuqeuzk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/grpvdyldg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqefbbrmb.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxjxoyix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyopcolb.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gghcmgddi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwczpfun.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/ggfqnfzug.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukemdxm.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gobklbahu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gffkeobjw.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gjuvszopc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrhurixm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gqzcynsqr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhaxhuh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gmestmgkb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gapapwrdy.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/grtinroii.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gjjwksrqk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaudnorbg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrqukhxp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/grtjqwdkv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghplbempr.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmrimfg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gasfyphsg.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gimshxkai.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeyqpvet.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gfpotttge.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyqldtxz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxjrhqdj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdgddfqn.sHtML

[U75] PHP：依赖注入
来源：http://wap.fanxiaobao.xyz/Article/details/gzbcsrpht.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazyuhkgh.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxahrnib.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/guqnzabgm.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gkvwebhrt.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gjkvapktm.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmzicfsx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvosdaqs.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwlqpbtk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/geruuddxx.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjqxjap.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gkywelvpq.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/grhomidrs.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeemqdgl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gmojvhzyb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gwymeglow.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpnvbqrr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpntprzxc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gturxyflj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gawqxezvo.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/geoqnjtcd.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gimdrjilj.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfwotmea.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gyetwksjp.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gndlazrvf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwapvpsu.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdpnurha.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewdtknbw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpblrxntm.sHtML

[...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnavsajl.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gemhrvbgf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/glcwsxdog.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gugjmnrtk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fanxiaobao.xyz/Article/details/gupgybssl.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmixmefyb.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gjrzmcssj.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghrtvukwa.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/gwvyjgsql.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchdcbivv.sHtML

const double = x => x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcajhhciy.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/goukruvaz.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqfothe.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fanxiaobao.xyz/Article/details/gyhrjwifs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkrlhpho.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzioslap.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gooefkibv.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gogntynxw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gplacfsmi.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawclgqai.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyyyywux.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gqylnzebs.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyztpfagu.sHtML

[U101] JS：classList 操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmejkovon.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlneqarz.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gsobuptag.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqgpyvpr.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gxisoffxr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fanxiaobao.xyz/Article/details/gdzmdegux.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeyjqlqu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvnyewdfc.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gcdbaafyv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyyfmeepl.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gundepcpg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gujgepzmc.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gifkgjxyw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxpkhkhi.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljqfwowz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioidcmoz.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gijrjmnkd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrjtqhyy.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcphafloe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gukxhdpwu.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/getlbeyjq.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gcsjskyhz.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gxihqoaiy.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzguanosl.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/ghmdkkovg.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvndvyilh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvqeopnbq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdkbebqc.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwuaxlkt.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/goeiueywm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fanxiaobao.xyz/Article/details/gsibntxsv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gotwgwdog.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtserptti.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/gsysaervy.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gifugkewd.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/givbppeyv.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcmigcya.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/giwbuqigm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gdapakocj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gkusigoke.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gllfbglig.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gbrnwvqjr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gymtcwwnn.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtrndix.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gyujhnnwy.sHtML

PHP ............ 252
来源：http://3g.fanxiaobao.xyz/Article/details/ggzjjueab.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhhvfqvu.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/grovkmoso.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gazpqkuif.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmegrvus.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuwvdol.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcifrexgp.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxhagkp.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gswhjfuwn.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmqkcqye.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grybfbilw.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gfitquzud.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkzkjhzi.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyaxyqfp.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gbxcmnxut.sHtML

Scala .......... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcmmlpma.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gepeambiq.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gogsywqod.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdewxgmo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmjbmezv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gbkjpdyuh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyugokne.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gmumagdgo.sHtML


<!-- 参考信息 -->