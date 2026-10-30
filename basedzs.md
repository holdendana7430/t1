代发 wailian999

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gthkxclpn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gujrcgmcv.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gsuxnnhwg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gawiwsfjp.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gfarkdubu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gauvrhqlg.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqpyeznjb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gofybsjib.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gghsfcelf.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gnxjxiiia.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/guxiehpmc.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gxwwwdxai.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gpyvqilmn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gplbszhss.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtaimabhw.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gstwjpqdb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtkjmmrln.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gantyhtcj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gphdtozym.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gugusbnjk.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfnxiazmw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ggflmmzyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gaashozle.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gjkooatbo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gsthzjear.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/giodcvylq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gfyhqmggc.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gxabgcqds.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gfegzaenn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdoibntpo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gsflwsqku.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfybywebo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gatqyptxn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/goutfgkqd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gnexuywta.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gzfonxlor.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/glfcxbuvb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gfdowgncg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gukcjmors.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/grlualnji.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/glwtpmvgd.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/ghijzqpaz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gxkqcaetf.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gibnwbtjl.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gbqpswupd.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gzwddxukt.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gzudpgdnj.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gzcvlquvd.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gkcebhego.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gutrqcssd.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gyrjambxc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gjhpwtpjg.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/glcdgycwm.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxnbcjzk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gktyrkljq.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gnkrjooxc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gybmhnjyl.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/grxsrvymw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/ghvzkbpgy.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gtwhlvtvn.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gsqohafpa.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gwrbougbc.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/gdbfmatjp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gciagjxnl.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gpqpbvtkp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gsbhqxopt.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gvyqzpyrl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gexitzqcy.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/gvssvprnb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gnmwtcxlq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gohhtdqyx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/grhxeioyu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gprpdrpuk.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gsbudnhxe.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gweclguow.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gnzyitswk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gcvsbhodr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gcefcpowc.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gfsshittj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gawuwsyzd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gdzqrgzjn.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gtvjsmbeo.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/glyexhhcy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/govocnehb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/grcxvtvbh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gcjagelra.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gfpexxwmw.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/guawihswn.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gnsurmupi.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gpaejusen.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gcoduhrko.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gkkbcxzow.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gqmajcwnn.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/ggqfvfdzo.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gjeyglhqj.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/geucmbjmy.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gwjcblyuy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/grqpxuevg.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gzdnfpilj.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/guezalbtn.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gwsxqgjeh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gtarfhuxi.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gvklkqisy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gvmdtaivx.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gcybsrmqq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gstltcetq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gcsbrgdkh.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gmxdcuybc.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gabcoclya.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gvwpsgyhr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/grxspwfjw.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gwrbsixto.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gjwykahvy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gyedimuyz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gfbtcqtei.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gbncyopmi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/guygqzacy.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gbnelrkzo.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gzxqmqmdb.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/guvabugeb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gjgyzooig.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmhpmvova.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/grlxnysts.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gwpqyhyil.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gmpnienaf.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/ggeygrspc.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gzonpmaza.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gaqjscunr.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gwgxqohpe.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gukhauwgj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gaxiukbmv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/geunxecif.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fehbvm.com/Article/details/gfxugmllu.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gpavctcek.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gfymeqbab.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gtmynyvlg.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gapocazfm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/graiphrmp.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/goloinksz.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gotlcsdnc.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gbirdfrrc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gylzovbhp.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gjkbakxvh.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gcsgdhjbd.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gpcrwwgzm.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gxamxwgnr.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gxjjncfnr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gvfwubovi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gmtjnxphk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gtpdazfmp.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gugrldezd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gbtuhjfkh.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gxqanwyaz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gmnjvjuyo.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/ggghdgnvn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gdifmipdy.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gtdbxjsac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/glorutmca.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/glcngdqww.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gxrznybuw.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gnsaqcoej.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnoigmxck.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gsehbjoex.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gcoaymyky.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/geykkwmrb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gyapmjwws.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/ghvrelpqs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gupjmucwj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gwlfapygc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gagytcnfl.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gblwckacv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gjqdmhupv.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gdhggbvmr.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gvxvqdsjb.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/ghckaymyk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/giledbxpb.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gatwklrab.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/ghqvkdyjc.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/ggwcvxang.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/geycwdqkg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gacyrspym.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/goxcnfcad.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gepjjajpj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gangixgby.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gpdnewmqf.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gszrwxgoh.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gjibnzypr.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gbczkyqwb.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/glnahkomi.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gfawfyslr.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gpzgbchnb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gswbecyaw.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gzdyubbpe.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gxvbqbmfh.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gtuttbcrx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gzjzaaawg.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/gsxtcqcau.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ghhcmjmti.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gezclwnfy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gancyqoxp.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gsdbvslmm.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gbzioeytp.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/glpivfaos.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/gxqoqpqlm.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gbynbrrdq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/geruigfbl.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gzaypwrqz.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gyaepkmqa.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gyqihluow.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gxnninqah.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gsalqvhts.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gczxxqixf.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gftgteswz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gvocrslgh.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gjfctrelh.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvexmvrri.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gnrjfxxzg.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gitjfnrrt.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gyrffadko.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gxxxjfepg.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gvpdkoptn.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gtzvzmyza.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gaolimkhe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gjkgimyyf.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gpgdamxoi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gotzbfpii.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpuytvf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gpxjlcysd.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gywdeqptp.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gmxfsvate.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/geanlldrm.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gxyzgbcel.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gadavvsmc.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/ghwixijeu.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/grirjfezj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gisphgydc.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gkvvjnogz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gbdjhxglx.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/glktbbsqk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gsiezeygz.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gylgmzask.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gcacnbekp.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gzbuddndf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gjkcwetam.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gqcyhwvzl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gipnshqcw.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gtaeodhdw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gxmzfeqjg.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gxltqbrjt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gefjnmzva.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/ghxeubwar.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gtybkkyms.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gqucawyug.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gcmfpzbbo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gdyydurbk.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ggwihlxmf.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gugrkhscj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtabcluac.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gzagvdynv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtumlckzr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gfwvakxxd.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/ggvqftioi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gdsjcvvzo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gxlefbnht.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/glmuciblf.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/guucnfdbr.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gaylkagto.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gwpjosqaw.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gaerwbwvi.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gpdiutxup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gwpttadnf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/ggzdxerqc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxuklxhnc.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/ggggllyam.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzfgqogmm.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gkxugqvfx.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gmzmgkupi.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gndijdhfj.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gnrkcwbwm.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gjbonfbgr.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gxkaufbpd.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gnezntyyt.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gqibbriqk.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gdpdtuxlj.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gxfqneitk.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gpscquwlv.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gppjbbkhz.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gmepccxzs.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gsloegzyt.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gppblfbtw.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/glndywwcs.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gtrlxhjwf.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/giadpfgpi.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gpuqpvtei.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/ghbehqwwn.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gqyonadgg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ggjlxymir.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/giifvidyx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gigpbwocv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gdnyqrpry.sHtML


<!-- 参考信息 -->