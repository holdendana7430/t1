代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/glriiublp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gfduqwmbs.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gjinebvjm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gfwzvgujg.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gqqkebuwl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gwquzdzyt.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gfdlhacoj.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gfpsmkwqu.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gmfiiwvgv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzawryrej.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gyodiacgf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gkvvyuobr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyzwtslc.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtlxubawk.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gulqwfizr.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gjcirhemj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxhsmjtow.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gczbfsyai.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gxhuplofv.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gtujzspno.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gefimispv.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gyurcyqsa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gwzhrauoz.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gwdrcljig.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gevczeeyw.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gecyaugcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gnkhkpukh.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/grexrglkj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/geulzypbn.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gvhusctpd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/glpzmdprq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gnjfhssyw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gnptpjcqx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcciipqbj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/guebujuwv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaqhtaqcr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/giytylndf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gzwakochw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gdcjsbwvc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmnguvudn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gnwswuier.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gmzecvitz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gusptctgq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gtyzfdhgd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gguilybwz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpxcnouzi.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gjenpfaeh.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gsjxthdyu.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gsgsbnvsp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/ggtbumgva.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gcemkmpyp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gyxpsrpsx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/ghywzmsph.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gehekwwus.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/ggyxizrbg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gmmnvhjnu.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gvqqojvnz.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gdnlhyxxa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/ghasjjfwm.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gxfaejtbt.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gxmkfzqit.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gpovnobpt.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gtfqiburw.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/graybhjtj.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gtzjoddkj.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/givpohwwk.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghnnxljge.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/glinsxllt.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/ggsprnaee.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gvqyonvam.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gjpgtekra.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gpzrznjqn.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gpedywymk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gecxhgsop.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gqbsgcxzu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gghioabpc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gxdbrutnv.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/grnocnfdy.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gpnlynwzk.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gxyoeburg.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gxcoppnlb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gfflpdpew.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gmruwytmt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtljxwhak.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gtudqeusu.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gzhkhebfv.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gwiqccitj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gpjxjitnw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/ginymwxdz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gkppayifd.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gmbjzxvde.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/grjyjceml.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/godysndlg.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gfwygiwgf.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gbbzbbnyx.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/ghljkiqlj.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gexxogmlg.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gaohypves.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gkzqezgcy.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/grsigxgha.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gxurtzxkf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gusczegoj.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gdzwsobca.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gsnycwtcw.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gsxmzmylf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gitfyeisr.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gcvrbynnb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gpaaacltd.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/goeecwdgm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/glmnkerxk.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gqukfmpxn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/guinqprdy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gqszhrcek.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/giyeatafr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gjbutbxly.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gwvcwmcql.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gfjeozjxj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gdprgktlv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gpyftldnl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gbzsnnpif.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gonipcmwt.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gzlxqnpvq.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gyjalxevy.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gftnsuteo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gweuitihi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxpxfmoqe.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/ghwisbomj.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gyfounnbd.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/glqentcru.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/grokkgziz.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/geuygvhoy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbadwnptm.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gqqdcjpsp.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gfqjgpqhd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/ghbznxjfh.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gtfakfrqy.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gouasrzvu.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/ghcjkuhet.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gvsemwamq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gpjuhpoup.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/goqyyprds.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gcaoogcjp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gtkrvxoui.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gywqxcwzr.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gcykdwpey.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/giccuqkry.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gkxcywzoi.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gqdjinjjb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzpcjhkdq.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gljyfdhqc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gqyyzllfn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gaubbimpe.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gltsvonft.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gnfvwaxho.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gdcpkgxcx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gyavzsmoc.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gbblrykcg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gbqawmcvb.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/ggruqjtzr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gdghmeddg.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gehcpprhd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.hesvh.cn/Article/details/ghdrkskct.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gcuvtksac.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gayarikhw.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gzjbtqfba.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gimgwiqjm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gyornmekl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gslytbsil.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gwxacgdjt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gdmfqahzw.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gcxqvkqew.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/glimvqzje.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gkdfhdtxx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gfmxxtunp.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/geatlxutn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/grwqulghs.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpressb.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gqbetamdw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/grceyajzw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gppfvljak.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gskuzvjil.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gtkavnoyj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gvepbzfhq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gfmiwwlbz.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gzkzoyacm.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/guoblkmsd.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gwondvboy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/giwhigecz.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/ggxfhocde.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gxiafklsq.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gtrrcbsaq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gdidcwmmx.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gsiygmttt.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gmtpgpckn.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gnspzmuvq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/goywmsrub.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/ghihmkmdh.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/goxermflc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gizajjqxf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gjeoksroc.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gdeyngoxv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gzsodtxjk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/grcyxhavy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gdyjgbkhs.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/guoyiodqx.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gxnsepanw.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/guaeyrmvq.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gxmzvshhs.sHtML

[U87] JS：解构默认值
来源：http://www.blog.hesvh.cn/Article/details/gqdtkwnmf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gawkedhcf.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gzmvuldyj.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/giqkkrzcg.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gtehougzu.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/garvoujke.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gkihmuqoa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/golsfbyrr.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/ggqofjjdj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/geyqjwcbs.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gkoteumih.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmbiqixzp.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gdopysywb.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gygvhqqbn.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gllgumzrc.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gssjzfrrw.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gmpbrlvqn.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gjglspjmb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gamavinnu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkknmlpba.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/glzmxesfe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gxgixsdfi.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gtqlehxwm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gnqykwsmy.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gfcsjbviw.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gpdpigrjt.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gxrrxcbva.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gcwbhmggh.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gthyvjqoe.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/glhkqgthz.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gwyjbmzvl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gziatmieu.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ghwgesskv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/giqiefyid.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gsoxdjdkb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gabdjqcyb.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjlczci.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gujkmhatr.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gltqjvhnp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gtxhgbrex.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gpgyifege.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ghrmlgggn.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gjjitkpmi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gvrfhdxys.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gxjbcofas.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gqnwsmoyy.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gymwhgnql.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gbzmaazwc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gjpnfaskq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gltzospwd.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gkhpgtveo.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gpqslhgfs.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gupogpzcp.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxqwczsam.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gyjnotezz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsjelhvbs.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwivgkhpj.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gtwagjntc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gfjxjyzwi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gngfrxzqv.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/grwbslewz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gxdvxwwny.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gyeutmnpd.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gknicieid.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gzddnczfy.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gohquylea.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gpqqjager.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/ghjjsvgir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyqdvrvsq.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/guejkvqhp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwqykvwwl.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gbhgoplkq.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gehlytnjj.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gpchvteai.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gcmhqywih.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gobnyqcbw.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/grcumqxyk.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gapysqhjs.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/grvogkvey.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gzcuuqqeb.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gguzirrzj.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gtesupozd.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gkxigyboa.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gvxujenep.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gkylsbrud.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gyannbkgh.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gwvqdvydo.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gdrqnlkiv.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gwmxeyyha.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gncdbytdo.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gssoguwbt.sHtML

按章节统计：
来源：http://read.share.fehbvm.com/Article/details/grguqvsic.sHtML


<!-- 参考信息 -->