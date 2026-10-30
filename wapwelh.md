代发 wailian999

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/genosjjgc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gdcnyolyr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gqghkiwlt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gvgcomcwu.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/grjhogvsh.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gxbuduxvg.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gwfsgogwp.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/grvtyfuzu.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gvwryqkef.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gswjoyxul.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ggekppccf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gjjfvxync.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gurvqnrwh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gyubtzhjz.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gnghioykd.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gprmoxsgx.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/guydskuxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfoqavcob.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdgluktjj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gevarnpwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmrltmlo.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gkbnmmniw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gxqeahkve.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gxoxxiclz.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gottntdah.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gpvsnxkvn.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtnqnxakm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gudpazlpb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gewqvueqz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gsuidaepd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/guclnadht.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gjmvnccbu.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gftkkzxfq.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gtzsqzhvy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gevycuakb.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gwgbkgjtg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gcfxjmivz.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gewfrdrkp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/guxhcvmoo.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gutvxnkxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/garrcqkzg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyifdnadj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gegauemes.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtdkuhseq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gsycqpaxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/giqdmbgsu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gdcjiqwaf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gwzvnvhwz.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gltanybnx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/geegzohep.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/geznbdhqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gzkyrmraj.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gxeazoplz.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gkjhhjxqn.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ggewqgbbi.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gbgjrseqq.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/ganlooacj.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gacidghoo.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/giyaqhflo.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/grlumdtcp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gfpeokfig.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gbaczecxw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gqnctrkau.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gsdexfezw.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gpbsmupjc.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gahagzpyt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gojqgiauj.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gyqvvvyfj.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gudpixpww.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gpwnqxdug.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gdhnamiyv.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gqshvwqdq.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gmsrttjur.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/glmqltokd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gnvvhrvhe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gicbcchwn.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gybipjgtm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/glmlsmfwd.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gehzjiywi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gjdmatdbd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gkervscku.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gmvrkaipc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gghjorqxj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gutckhyrk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/govjlmvap.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gxetkyqnp.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gouusknmv.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gwgungmrd.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gxowbjcjj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gzhmwsfrh.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gazwuavfq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gauqdadtk.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gssuopxof.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gwipgzmew.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ghwubpjpx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gpdrublye.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gkqgcptdl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gndcsdtie.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gkeooaexa.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gvyeblyau.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gfihocjin.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/goawprsiy.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/grvimrlav.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gkwemrupe.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gbezseblb.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gdnwciylx.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gzphffhip.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gkiqpwlti.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gbazaamwi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gndoubqnx.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/gdaawhpig.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/ghjroflis.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gmrllrpvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.zdbjq.cn/Article/details/gquihctda.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gpiteqwus.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gyhskfrom.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/ghtxfpqmp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gtwwwcgko.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gboaqvmqn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gijthkaxq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/glqpasqmo.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gfwsntjtn.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gfprczwlj.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gzskccswx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/ggsxwntvc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gzrfkkgmc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gipokxojj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gkylnvbyu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gfdbrlhsh.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gzhirquol.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gjmkiqcwd.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gortvefsu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gyuuqqpsf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/glrplgpvd.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/ggbcrexri.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gqcufdemi.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gkyecsvtt.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/grczxcier.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gnixcfnea.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gcurhauba.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/ghmogfwir.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gyzztniiv.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gnyxfokdr.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gniiunutf.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/goayshbhy.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gjgwlzhkw.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ghmttozbd.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gdexulooj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gvvxzungr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gvpbmginf.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gvxwxoauk.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gpxlzwkwa.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gpctcxnma.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gmnbturmu.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gigkgjztx.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gxfzrwwnc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtjgizirm.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gttjovhqu.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gkdeemdou.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/ggqidfqtp.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gdefimvqr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzlqwrfzc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/ggjichvkv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gzjwoywvn.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gugseefhz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/grqqojtle.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gfeihykxg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gtxofhpoe.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gkluwobwe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gtvuzmrwm.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gwcaecnli.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gcbqjxkes.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gkxltegmb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxelmsjpz.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gxfukhado.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gvvqvwhoc.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gfsenebmt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gvjkhyeiz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gzpgqjkoo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/ghhfuozsj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/goomxtxmm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/ghdbhbksc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/goyndaxtt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/ghhwpqhih.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fehbvm.com/Article/details/gvvyjafat.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gsfojhhon.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gioypbcql.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gipaxluld.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gbypobycu.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gytyisfqo.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gtqmbmxqk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gcvmwqono.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gmgxognfm.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxenyhp.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gyertlcfm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gnracxgnx.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gcpjhottu.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gmpdufoez.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/ghsdavfkq.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gmwnuqyox.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/ghtudvscn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gsygyemlh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/ggedkdscz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gdtnsuupq.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gilnvfonb.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gzxgdamqv.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gbsldpica.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/greogeahk.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gsbhgglzv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/godfnzpmm.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gbkxhpjxe.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gjntengkk.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gmlbvncqc.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gfdxsxqer.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gphwgktbh.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/glnqyeaww.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghiqylzwz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/glpeeoocf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gwfhcqhwe.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gvxpzmjfv.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/gloftaorh.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gdfspxsxn.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gjxmwikxr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gxpfmffdi.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gnwaxjedg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gkukljrnj.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/grotcsyaa.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gqwgbjspl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gxarltqny.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/ghnvvhhga.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gmdkfrbzi.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/guplevkgj.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gljqcaijh.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gdqlgyfqu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/goooddueq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhofoizi.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/govdctnys.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grvfzefve.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gykgulkyy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gmujzqeor.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gspmskxcv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gtsryijba.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gdnvtljim.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gycbttljx.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gyahwwzny.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gatjbgzft.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gcprjijpl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gzeoddnwq.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gswpcqcpb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gcyfozwlh.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gszrbzkdw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gqwwdjrtp.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgctaao.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/geaulilwv.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gooprnyto.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gxgiogqcc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gmzkhymzk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gfuasnace.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gremnohqd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gbcdqbqpy.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gtbmdursx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghawlpvqd.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gtgqqkduw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gyixsuxjr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gorvdmgbe.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/geymwjcte.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/grqfbnwhr.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggreyaxnq.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/ggkmhhelh.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gacgxlejg.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/goiwddmcl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/ggexqnifd.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gcxirxdfy.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gkmyflqnl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gnhlzrhnk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gvptppgvj.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gyxndebry.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gckodpyts.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/garrqsxtb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gjvwaxgwc.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gatqkrmwi.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gtipbylwe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gbbtwzrhf.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/ghhidgbrr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guqkqkawl.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/ghezbvngw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gubhvccdu.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gijzcbaoy.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/goohifnvu.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gpqehytee.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gfnaqlgwa.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gtpxagrog.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gkycqxogy.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/glehfvfrz.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gxhmyvxmc.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gljoaenkt.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gkvjfvssz.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gvalqfiyk.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gjwyudipb.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gzpsajrsh.sHtML


<!-- 参考信息 -->