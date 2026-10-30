代发 wailian999

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfwppjzd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfgcrhnzh.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuothlwl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgnnxesu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gajbgfdot.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjtennetn.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdjtncy.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gifoyjzkk.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guuhadbdb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/glvagjnct.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxampatx.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeiqgumn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvsmdzhy.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gefdqdilm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnhlzyfw.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjvfhojy.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/ggvnumalq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gloritysx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvtqwmqx.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/giujjxmhg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcqpebfc.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gqjjsrywv.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gyfrzctux.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadsedpaf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gbdbezvkh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszivufg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjlavvth.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gchjqzhkh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqfrlvib.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciefehpq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gpvzmcjdi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gltsqduws.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhkgfun.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbtekoyt.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gdgrtoyhc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyzxevb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbgszujc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gavutxjzj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/givejajps.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqxsaxn.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gjnlggoxd.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/geqdyqhno.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gucrozquq.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/garrznfgf.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gaqrgmvvu.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gbzgdmapm.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjgovqma.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlozqqhy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gilnjkycf.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gndrjdqjs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpxicljae.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gsbepyopx.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gvpauaxmb.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gtbykfcxv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gelodljid.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvhymnxj.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gdqfnejmo.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/geecybrem.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gxapceliv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwnszlxcm.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gmvfturxh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuxcyjrk.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gtkbtgtze.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyaaonli.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhlcrlfk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/girrevojs.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gspuckupz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlqemsxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gccnhhxko.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgynsjor.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gtavapxyg.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/geoyxjotx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkjemnvnv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjtjkmpk.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gztxpokns.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrdrzpqp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljusztyx.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsjqsqqg.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gdstwzcbc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gtujqsikn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdjpuuwu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gwlwqudxg.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbqlqjlu.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanhekmv.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkcshwrg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkmsaaq.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtjblohu.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/goyzkjila.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gaqifnuav.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxrtvrgi.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/glfsddcwi.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvktgce.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/ginnxgtcr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkuxnwpg.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyknisegq.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gworwdons.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxmtumab.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gyicdveaf.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdcaygbd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/grkjhgydv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gggvmhddi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/grkeajwlw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbtilbvb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkcemmqq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckclaijq.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gceoijzli.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gnffryrpw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gyozkyxjd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gisfsnhwn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgzliqln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gresfwgxh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggazlisqp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgqcegb.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkznttth.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmjeczyi.sHtML

declare(strict_types=1);
来源：http://3g.fanxiaobao.xyz/Article/details/gzckrfvfc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqyaovpzd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfmawsimu.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfpojtxjc.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gpexiplvy.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtmstwbb.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gtahhiteu.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gnizzbocq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghllplvgv.sHtML

[U49] PHP：只读属性
来源：http://wap.fanxiaobao.xyz/Article/details/gvcrzljyy.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvkfjzpe.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqubgsx.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gokrsjamz.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gctmgtuus.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gwvvuuzyk.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjktcacv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gvtpbkuuu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gyiktlcvp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gibfvyjor.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gehmhnbll.sHtML

$obj?->method()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiajlbvq.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjlfgapaa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fanxiaobao.xyz/Article/details/gkejsvhdw.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkhuvnjv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwpjssad.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyipqdvv.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gackioqbl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmhgypp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjvzahph.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaoqoued.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gmkbvewjf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvpcjkqw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gflqzmlpc.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gljifruqr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaturiqyy.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/glguwxsrc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvzzpql.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczchaxac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeatmfvz.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gquxyzeyu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fanxiaobao.xyz/Article/details/goozrzpeu.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojghekgw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/giuunduoi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gynvmfwdz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhyvsaqp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjnsxio.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/geazfrpkk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejbeuvvd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfqpzsuo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcxdnfbit.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gakghdbji.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlsxgvtg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/grvdwqtvp.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gpubzjngl.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoxbdrje.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduqhxugj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxqyvnsj.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilggetai.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvubfnpo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdvrwiup.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/glepfeipn.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fanxiaobao.xyz/Article/details/gxytsldpv.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gfnioiamc.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqeqyzx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuvlitlr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gegmzqyum.sHtML

composer require twig/twig
来源：http://wap.fanxiaobao.xyz/Article/details/gvlpaeqlv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuxwlkxc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gqorbhotq.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gksdjxjxk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gljktejxi.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gjyrxhgqw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnraeonr.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggofygbtm.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/gwanyebrd.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoshvpsb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbskbyafs.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvxyusfl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrbfjtzp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnowrrgkk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjsemtr.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gludyuhjh.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpsbrlqh.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbttnzev.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gqbkxxwwf.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkpcjmao.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumtlecvg.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gsncbkise.sHtML

{ ...a, ...b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpvnslki.sHtML

[U89] JS：数组去重
来源：http://baike.fanxiaobao.xyz/Article/details/gudpjucvd.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gszjifnbu.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscqdpove.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzeeympj.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzsuipywm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqxmboap.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmsnxmlk.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ggveykyeo.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbozoga.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafcdnjyp.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpjkdxjko.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjknrujt.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gswddhvbx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmybpqrjv.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxhkeitmn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/givwpghrk.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcupbukh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnowrdmuh.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnkrfeimi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtiizdgx.sHtML

[U99] JS：事件监听
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtutjulj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gruxihcav.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqspppgv.sHtML

document.querySelector(".item")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmprdqvw.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/ggpbvhcbx.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gwkpeldyn.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgqrernv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwborpc.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/ggmggylwe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrgbmrzt.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gfsrjhqsz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/golqltwji.sHtML

[U105] JS：节流
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeqqldsi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqpomrah.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdiinqlzp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gyclhuixw.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gziaywrto.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssdnfpeg.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/giixifkpo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/godqigapc.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gqguqgzgs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/giaihilbo.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gqhymtnyg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuarfbhv.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkmmauzj.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/grcwgpllr.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gmzithymh.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gofhcesvn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqywmeh.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gpnixljtk.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmhleiyg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/glboygfso.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gseaskjjv.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/ginorzjkx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fanxiaobao.xyz/Article/details/gngnqzyoh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gewboisha.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gqbogjbqk.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrlhlhvw.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gxphghqnb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnqmbnfv.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcwspaoz.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gnuvygkny.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gvgrpdofy.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gofpdsxwi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqtpdtxkg.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwieajxk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnmhjizo.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gpspntllp.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgifvune.sHtML

PHP ............ 252
来源：http://blog.fanxiaobao.xyz/Article/details/glemqqclj.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/grhjxdrym.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gwekrrbso.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/ggnetanqt.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/guolyvqzv.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfznytgvm.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkydasiv.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzeonkea.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxipxgzva.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/gixeyvnfs.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotiggxpc.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/giprwthbu.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gggaaevyi.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gznjnwoic.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/ghghgeudg.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gtrjxiugv.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvfkrchu.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gzgkkvhfb.sHtML

按章节统计：
来源：http://www.share.fanxiaobao.xyz/Article/details/giiljkmvc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gtzoaaqfp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/giorghfxb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqpkaypo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gliifyaep.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gokdmnfst.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsbejan.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gglpbliac.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gurdpmuly.sHtML


<!-- 参考信息 -->