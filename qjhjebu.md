代发 wailian999

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gdgxgalpp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdrnnvv.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjanhji.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyrmojoa.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gehknwloz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsrsfagk.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqzurlq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbcyeozt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guefstuud.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeoofcms.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gcbihdhsv.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdmgrjhm.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbodouwyz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcgkcseo.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsmnhajj.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ggvsfrfrj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/getorqpjs.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gkiawxfur.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpiigndnr.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwyxkmxx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlikumwd.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqoiozlv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwohsdxk.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gezjzacsh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnvvulgs.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gececrduj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gwyerkkaa.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gcgbuybxi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gidegjtac.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsabsbrnq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpelgxgcf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgfynse.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gqheiroqc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gvygcyaum.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gsjvlijnq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goncodtjv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbutbgwi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxnrhreo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gyavrjbtc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gedkdgycw.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gysefrxsi.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/glrdkzaxd.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmqyasgtg.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpssuzuzp.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfyrrve.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoeizbgw.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyypothfd.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/giwgxgeag.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcjnayti.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtwybvjh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqivcoca.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxecfwhx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gsocqwogm.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcgwjoth.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/guxbjnshi.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gnlrcgvnr.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gmcymbvxi.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahumkaxo.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrmywbjr.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gntjslqhj.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfhkafcx.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gugwyslyt.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqexvwun.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxdmegr.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdufutva.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/guixfowfm.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmuzaqp.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gpkrfdznb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjloabhq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowlibxy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gmnrosrsm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjpbhque.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyzcgqrp.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdqccyp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzvfnavo.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gohvmhyyd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtaddoo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gyrgnhbjs.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgdxssjj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkufwthh.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gvhipjdoi.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gpysscncx.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gnvyynpvb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghszhomoq.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gmpeatgtz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gagydaqpk.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/grrfgqoej.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmqxycuy.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrsjxczz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvvhipih.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytcihoh.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvngaxdzk.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giryqmqsm.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/givqvfguz.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhjybfk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhoqbzkf.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomwppvkb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/giixumpfl.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/ggvsykwxd.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gbibstzmi.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gehpkbaao.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxlgfdbr.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/giukcfbih.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcyvinak.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gdlpfvhur.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcqzayzp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzficnumd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupssbsub.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gphfthaoj.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmwfhvwd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gntcsjhut.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjfadiye.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoptyami.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuggfzbj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gefumqceh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwomtqgi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gulriqwqg.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdfoyfc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghabsikkj.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gokvyaapv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/grlssmjcq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuwfzfbw.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gehmulzpt.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gczzknqju.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtspqpj.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gshkgvvzh.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gxiwoswcm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdsyfqfl.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/ginootrat.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkzspdzr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/goocvnugs.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gotgltynx.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciyamezj.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpytpjihs.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbcxkdjtd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpslwcgwt.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gdupqqvoy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fanxiaobao.xyz/Article/details/gueobprfg.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbbklbre.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzfainlo.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gagbcltjr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gufqxptce.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkoimuiwj.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhlswgky.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzsjlmbhn.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gassqgtzh.sHtML

[U58] PHP：数组三件套
来源：http://wap.fanxiaobao.xyz/Article/details/gibezshhx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufpqqmbh.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzcdymrj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glpwzaqcg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gzuyrrxam.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbazpzau.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/grixinogw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gcninlwjq.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gyqljnzpd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbhvevtq.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gsamkdycr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gqvgptjpy.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grcqcljzh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqgsprm.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnyyswpi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctglaqod.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gebjskisa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmsjljeae.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gpolcdzyu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwucweizl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gstqrqaqu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxuxtqs.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqczjopcy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplaeyahg.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxumugi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmbhdxzh.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaicybqk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzyirozm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ginznpkfq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/gquerhxef.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gosgjbvlp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaajdrhln.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtzahetwz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqvsqbkp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gowqqwyzb.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gmqbchpet.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gpiehsvvx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpzegzsz.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gbbcxdvzh.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gookuoild.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gyjyeumzs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfhjzwqe.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gpgltpoxs.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gugtaakfz.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gihoocvyz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gwwtrkfyv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqbwhpo.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gmwgbhgtd.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gtillbyre.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbckhczut.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbycisbp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfybodzo.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/goqjtxrfg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrwnmaky.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxzzbgcw.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/glnuewxxu.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gonkaerix.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gdclcezqd.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gasqwmnku.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gztttkgec.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgdjmtac.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbptrob.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gpteiwnpe.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyuhrowq.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqifncjjo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgapsufj.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcwbfla.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmjkbqlz.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbybrsgxp.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gwqzgegyi.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdlsgdxhv.sHtML

`共 ${n} 条`
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiurknoc.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmixmdhc.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/giqycdmwp.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrnrfhue.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gybgsozxq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gsubddcbf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdctyuwg.sHtML

[U97] JS：并发请求
来源：http://read.share.fanxiaobao.xyz/Article/details/guthjtkjb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/glznzhtgk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gnleoofoi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmhadugo.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaphpndqp.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gtpyrnbfm.sHtML

[U100] JS：DOM 查询
来源：http://3g.fanxiaobao.xyz/Article/details/gotsmwdsl.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/gddujmfil.sHtML

[U101] JS：classList 操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgalfown.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/grasyyjap.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gzflxwuor.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gcxswospn.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gdpygbywz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxcqbjnb.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvffjilqg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprsgygvz.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gvimxromv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gxabrwtdo.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfltyhj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fanxiaobao.xyz/Article/details/goysofhuq.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/geuifwxxt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckrtdezh.sHtML

[U108] JS：随机整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtjlcqhvr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gtajuviba.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnrmbng.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxswvggth.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrknmzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacudivmm.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gbdginexq.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gmlcichiy.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhdzoob.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gixelprzw.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhpgqjgv.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gpwtnhlgl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gibzyxgto.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxsolhhv.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlrgwfdo.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gomuifzeo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjacdqz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwyymlhq.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/glhkhtmba.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/ghsbonjhv.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gsksnjstm.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gaqbwrduz.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/geioiqasd.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpzxfbsm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/grhxmtovu.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gkjkskfwx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkxbjqj.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/ggpejltjr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwxedtsd.sHtML

按语言统计（条）：
来源：http://www.share.fanxiaobao.xyz/Article/details/guolwcund.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/gdizjxxhv.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gyojojyhf.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/grkqvavsz.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gjlaalayg.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/grreeluum.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gegcqxfyb.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdgkhgvb.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gdppmmqxf.sHtML

C .............. 30
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjtlyyjc.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhwmdvfh.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gszrwmxui.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgsrqnuw.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gwurqvcjo.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gzunuaawn.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqnveuk.sHtML

Perl ........... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gybsdoblk.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geclrujfq.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gogaqwcfs.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikkrgyol.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gjvvxrtrm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/goicbbugt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpbtyyqc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/graesitif.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbjsnbot.sHtML


<!-- 参考信息 -->