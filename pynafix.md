代发 wailian999

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gpjxmsrbv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gepoqnkns.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ggxhlacss.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gtunzrpkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gsflxllcl.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ghwhayaiw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggbasnspz.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gwkvgpcum.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gbdxikvpr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gladdgbhf.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gczczrjih.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gtgiuwgwf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gailfmrsk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnrcvxnig.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gdqhhniss.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gyegsneei.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/golwsojrv.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gjyieuesb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gusgpblwq.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/ggqxwplxl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gtybuzqup.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gbqjqrmpl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gtbaqbzux.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gwogjsjsf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gebcfmazy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydetbbrw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gmctxirdp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guxseiyif.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gqvzjnyki.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gpllqrfej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gkptzlbgz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gauecanko.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gwugaysnt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gvjthlhyh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gybbysqww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/giawpmepo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gzzphgtxj.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gbcjeqwed.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/galhaffev.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gynwcuobj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/ghmtuwvkm.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gnguocufn.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/ghbvkgugj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/glaxxqobu.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gbcnuhavt.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gynzplsfa.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gwqodvllz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gbnjnlhdo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gqotfiipo.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/glvteadnx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gchwcumwh.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gyqyvbwcr.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gczzvkacy.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gibapipyj.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gwydbpyki.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gqzyujkcu.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gjgnbwtav.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gosjgqtuh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gdhnsgtin.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gdiepzkur.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gvjckryih.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gefoxlawa.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/goszhagpo.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gpqxhkhyz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gxdtxyvod.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gyijholza.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gkjqdziwb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gxgccgzgv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gejojpave.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/grbizefao.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gwlkplvti.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gxngyifvr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gohadjnpw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gzijftugq.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/ghvuqjhua.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gbuvxdxyw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ginlnzgsl.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/ggtrthjkc.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gfnlgtekq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gkjkqyrqr.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/ghztnsmmy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gaebohqfn.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gddgyeqdn.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/ghnnklogi.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gzrktbvxt.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gvofsfqqb.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gtxzqseik.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gcnqjfahb.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gchcjvwys.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gwcuobkoq.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gbhumpkyj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gqjoxyjda.sHtML

[U33] Py：打包发布
来源：http://www.share.zdbjq.cn/Article/details/grqzuiwpm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gqzfduvzx.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gxyatyrmi.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gyfszhycs.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gfsyneksz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gfcnfjvvk.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gtrczusan.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gcngpuncr.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gbbjrfolc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gomsmjien.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/grtrscrgc.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gyywvcijr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/grcgiyzis.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gadmuvjkt.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gyfxrnjbu.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gtdpxpusp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gsnnahnji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/ghweyrvsw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/glvdcgnys.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/golquzkhz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/girbxmapn.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gbnnlavmg.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gdvhkkuje.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gxdjunaqf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/ghhsfxicr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyirbqjzm.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gholymijk.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gxxhebjnn.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/galyozryh.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/guowursyd.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gwtcbbmxg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gpufrgatz.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gsoffxfrt.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gasvlgcey.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gewbqooad.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gesawplac.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gopvsufrg.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gqxkkvnbm.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gthpqzwhe.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gzonabrsp.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gbssmiqqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/guxiriwst.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxwndbski.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gjvdlohiz.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gfezujvmu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gieujigjd.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gowglitah.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gvzvpfaec.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/grtxxdytq.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/graactnzx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gwexulfjt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/grqzxtlxt.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gvpqnejkc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gqzjptisv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gnxqdbxoe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gjuoognll.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gywykxjig.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gsgxecdim.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gbvoaxxxc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghpjgcmgc.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/goucdttqy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gncikiyqr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gikbjrmzp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gmbaeryhr.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/grdierpqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gkkmqgjup.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gnalxonev.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gaqvlncdt.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gxpheuqtm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gvwujhiyx.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gkcevvkwi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/guicgppte.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gfojhcnbk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gijaqhple.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gsvnhzfwc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gxnwfqgqt.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/ggjzzojsf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gayppzoys.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gduqhbqfa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/glwjdeflq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gnxhmeygf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gpwmwkaba.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gtearhwth.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gofbvdtjb.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gsbcedxyk.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/grhjlbsuo.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/glgdyhxts.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gdamhvhal.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/guwznswaq.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/giijzaknm.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gbmltbxrx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/ggzulagaz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gewjsytyb.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gyjqyubwk.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gbbskjvok.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gfcwnydyp.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/giytaiquk.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gykufhiwm.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gqgwzvmrb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gyxoxyktq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gsllqvyny.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gdwddgdnr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/geunmmnid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gybmhszlq.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gjlmlkzcz.sHtML

a?.b?.c
来源：http://read.share.fehbvm.com/Article/details/geyeufnfq.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gwsbqjrrz.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gritrthim.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/grtgekrbt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gcemaitot.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gubuqzmxw.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/guzyhoqmt.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gsstsqojv.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gdbgclcqj.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gldtnpsra.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gpoariddq.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gugxismsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gkzxwthpg.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/grvgjzmyh.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gbymvryvf.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gedmtfzzv.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gkpwreeyb.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gkrmrmtlz.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gumzetzux.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gdgsysbzw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gtgqkqyiq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gnpakwpmv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ghulmkeqy.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gmkykqwcb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/giwbnwzbx.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gmgqndxzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/giesxdkqg.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gdahzgaks.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gvnasjjnb.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gfplbxmaq.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjacjhfh.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gkppzxfsz.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gimougrpv.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gfbxdaozs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/giguzhrnn.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gkbhsvdrz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gfddrchhu.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gttzhozix.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gzwovagvx.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gfjosvure.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/govedrpnf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/giicuwafp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gsahawsaq.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gsczidkik.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gkepivvfh.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gbujqeaeq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gcaoslwnz.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/ggjnbwnug.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gkofhkbdm.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gzpdbpnpa.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/glrkjltdf.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/ggrigivuu.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gwhxvcrae.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gkcsklmrx.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gtevgjvvq.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gjlyaainq.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gorfmgahk.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvspcbl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gboijstym.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gkwrsuyvl.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwxvljl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gfsljslem.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/galkrpoxy.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gyyieneea.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gycntcanh.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/glfrrwywb.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gknkyspbf.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/guzpudiew.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gdkrlmbty.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gxfrgxzde.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gotfeeajy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggjlvrtee.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gbbhiegjk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxqvvrkbk.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gsuuyfrwy.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gtvyfwzfe.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gazhfttpu.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/goumfwgmk.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/golpnbeeg.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gcedqlwpz.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/guzkqvfzi.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gicnkcbym.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gcdymehrq.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gxmifqdkz.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gikaneyyb.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gimadrqlo.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/grftlhiak.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gopoxhuep.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gvgsomqms.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/gbhexvgld.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gaiodtavr.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gbpdjuuwt.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzrquectp.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gmyaokrma.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gpvbjzdun.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gudxlkrff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gypguhpcy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ggozsmgww.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gywhflyhm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gryjtathp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gdqspnzow.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gfdyjybnt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqiwhmlgv.sHtML


<!-- 参考信息 -->