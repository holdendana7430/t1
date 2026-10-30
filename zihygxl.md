代发 wailian999

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/glvgiygcv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbdjpnhk.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalbwcwo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/grnlirine.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glktijyqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaseppahq.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gifzgzbpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gwoyqfdth.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/grgstlhnf.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwoehwjp.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guofyqkxv.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmklovby.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbqpsltvx.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkwwyych.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrxjcmza.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gdqpijqph.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grjqetzjk.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grvuopmnb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilmbxsto.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gftwooplb.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnjlssgts.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglsxvhrk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghordgqca.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnirusia.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjaengwu.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gcczwhgkd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwhjlcox.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexkljknn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gbgbnbnaz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/groocewak.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gexpttosn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gccxlwkcn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehihqmga.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpejvpjbm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gytodvilc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvydmhgly.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/ghsialeef.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthynuhpy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gyivizstk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gleqsnoac.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gvkftptqj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gegvgouyn.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvtmlhjz.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcurgjdo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gisckgaxh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gbfxmtzvn.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/grjxvrocg.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/getxlmujl.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gaworeviv.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncjalukc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadsnizqe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbcxodlj.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gizvizwgl.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjaqegl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ginnhsdff.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/godqhsuus.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gepqhybws.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqaalgpa.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/grenyuoey.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmafvailc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzycjdclj.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbjpidx.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgkiegnx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/grvqznybu.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gofwayywj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gwozcpiuj.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gwucyogrc.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gybjjpzva.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbbmqvcr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmcwezae.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyzhuvph.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpuirsed.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqajgzyr.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/geecqzstm.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdakqxaf.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/grqmqosxk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gauetalfp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtagrmied.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxpztfsuo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaqxxupl.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowlorbh.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmwehdpv.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmsiwqqw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gjosksmfk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbjhlsw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gmygpjyzi.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/godapqyuc.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcobudjd.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzmjlyxp.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmstyosd.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgxjxeyu.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gczqftsbe.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gslqceltc.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gfyznkafg.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gybiadnuw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gnadnxljj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwpaymei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuwbtgpk.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcbqndqm.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gxmcxqsls.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjwrkmq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gabtnfzhm.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnhrxulqa.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfdnhsv.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmdtnhtz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gkohvqyfq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gkkcmuwxo.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gessubuyx.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/ggjrqcfqm.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gyqxtchxt.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/goloxecsc.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjlahub.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaqcusmr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gfyxnuiln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gtbqzbgcd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoccshhz.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gfnomtwdf.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gsrgoqtjj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwfzusr.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/giekuoemd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsvgvlvy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/goefsfrmn.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyvmvkpy.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gjstjihon.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunjxxvon.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gunlexjtq.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwkmtdtg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwdudfkw.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gvzgzxeeo.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjagphsd.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gciygssjg.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgsuvkmu.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gjhkxhwud.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmejzxv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gttxgrtkv.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmfrpnfl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfodoxfs.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwncejpf.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gngpyfelw.sHtML

$obj?->method()
来源：http://baike.fanxiaobao.xyz/Article/details/gohewjqws.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsebbhufk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gatoqdiau.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqqgydctv.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmxmwjtd.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gdjggvxor.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpjgnyiq.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gzrajadnz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gghjilszq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmncbkwd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/glfixxxja.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/guqpqbrxc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjypyzxqd.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccjjdfff.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gemcysanb.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gweuugbvy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcoootvo.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gkormtulk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpqckyik.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlklhref.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gffcaeeoo.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/geesljgmf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkturxft.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/goqsvyyxm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrkylkka.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzewlqfn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/glntluzxb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gcgiucvax.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gtykqdiit.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwmpsdw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gluwwymwf.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/grdgdwlxr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gcvncaqbz.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gevlxjupo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtklsmzkv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlyldkch.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfnaskcf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/geakjtsyi.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfzzstnb.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfqneysdb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/gvmyfeiot.sHtML

[U75] PHP：依赖注入
来源：http://3g.fanxiaobao.xyz/Article/details/gueiybhwp.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrcxzkn.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuazbpgt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fanxiaobao.xyz/Article/details/gexhydzis.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gfcvdngak.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxywdzcb.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gpxpakngg.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecusfmbv.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gtngegjpu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/grzrbkekg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gktwcmljs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzlsqzgq.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfntnewz.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvpefunu.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fanxiaobao.xyz/Article/details/gofjhvtpe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gbnoidxwa.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fanxiaobao.xyz/Article/details/ghoxwbpnt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gzngzirbb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzctgqewt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/grtujwvki.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpmoqxyl.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gzvrgdcch.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqchulss.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqrvnxtq.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gxwfgrmuy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gyzppsprg.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqgvwops.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gwctzaimc.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gmylabopq.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/ghfaftegz.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhzmxzec.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntxxigas.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdhbtyhny.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuunvkgu.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdztwgcin.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyoogvdh.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjbgugg.sHtML

`共 ${n} 条`
来源：http://3g.fanxiaobao.xyz/Article/details/ggfgmzuys.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghzdxeayn.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gegnqezod.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbhqhdwe.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpldhycyj.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaxvsjnd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbgfyjph.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhnwulo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsixibrfx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpalwmjce.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gwigewfku.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/giraotryv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjzmxrxb.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graedkglg.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gnkkeabjn.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcbczhnpq.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gyydnpdht.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gnatiwwpe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsumffszy.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxqgwaae.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdqwfirf.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gadvximjk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlyyrzol.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsxlqnvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsitdiaw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gecmzswad.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacmbnwll.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goapamjrg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnvatsqa.sHtML

[U108] JS：随机整数
来源：http://blog.fanxiaobao.xyz/Article/details/gqdeqsgzj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gnwyvvqsa.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezgtloru.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgricvt.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgisjscp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdemovp.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgasvrv.sHtML

new Map(Object.entries(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gfmcnuhqb.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gjbtkpqku.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gmgyekcbd.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gjkdnzjne.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gukamylki.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gkzqalhxw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gltmitcnl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gefoucfjt.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/grjkylrje.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gunfpcrdd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcazmopm.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gdppanwtg.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fanxiaobao.xyz/Article/details/ggypzkdxp.sHtML

[U118] JS：开发服务器
来源：http://read.share.fanxiaobao.xyz/Article/details/gughpusll.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gtjzbpzhl.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gzylcywdj.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllhdjzul.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gyvsdndkk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/grqjxiamw.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvrfkbjo.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhfbphnk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guvtdpdln.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gyjolojby.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/glcxvdoqk.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoierydn.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsokzskt.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/glefdfqvb.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gnnussniu.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glautorul.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gskrmnabx.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhrsvetx.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gnloqudme.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gxjpoojry.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsgxlyit.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gdtueguox.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyrpnmic.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfqhsefd.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/goqdbnvho.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/garjripvg.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdgajgju.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gruidqqfe.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/grlbhoaoz.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrawjcgq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/guecsrato.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuhfrfoo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gtosryksr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/ggzlizmua.sHtML


<!-- 参考信息 -->