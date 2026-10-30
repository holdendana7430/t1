代发 wailian999

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqiedfmc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumtrzhbp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuanullv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqpqvdfr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiascldc.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxjgbmyem.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxakersyk.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxhczjji.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjychcyqs.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gknipdppg.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gwjvbjapy.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gcwptjlvz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtxkoyoy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gglvfkblx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gaslzgldo.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvspvtjn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goholrjrr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gstnfzbfd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkseayg.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gfivkhsds.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxdgvos.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpgetrbr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwqshvrw.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmiromiv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gqovugwbe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnppkijw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgldmvfx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfjnlmfp.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzouvyhp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfpvymtz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedicnxra.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwlufgnh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmprreiyr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gdnrrkkau.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gbeafbniv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzpresus.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gowxwohnh.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscezddvl.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/grwgfpzwj.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gtpbjqskz.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcdxficx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gftxfpvyu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxgbecub.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpbnbzbu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwzuophv.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/glcbijqsx.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gputhnivt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gdkjabqte.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gstoknygl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvgymzoi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/glhgivoxh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyadfnyfd.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggujljssd.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnavaokn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gdehbkcjc.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/ghtajemgi.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gnclkdkzp.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gaazmcofy.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpbppcmy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqwfcfq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevlyjeus.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcmrqhqo.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/glmlpokik.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gccpqdvet.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gpjyrdpyy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaxmvqds.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gshjhbwkf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfsgcrql.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/guctyzbbe.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gviilfyxf.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzyaqgi.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmrxpxtz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqtolmzv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gqkwuikmj.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnqmiyeg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqouqam.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gushjihdv.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gseexdivo.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpplcorqd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gzcjoietx.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gddhvydtq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gdgnmxuiu.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gqpivemqv.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/ggjrrudab.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkahizpzd.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklgnbkvc.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjlhzmzg.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfjoukhw.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/galdbqdaq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gexjbqobz.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrtrslno.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gdkhdacvg.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsupvpmy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttrhoiwu.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdymfyoj.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqsnmmab.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ghaqvrqwz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gabovmuuh.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxgjznfy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdxijutu.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gcczbfypg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gzgyizbwe.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gsjhlvfgm.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitxivlyl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gbjjumsnm.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gkafouaxj.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnhekgvej.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgykxdua.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsnvkvun.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gmatmkiwf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/gptcdxcrl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdrickx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvddskyg.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvslpeu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlhbtbl.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunnurexp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gomtxcxzo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvworze.sHtML

[U46] PHP：可空类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbtbvmqv.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjrjrpvj.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbhdplz.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyoqodrq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjtesbwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gouhxzazj.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjwtldbw.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzcvruct.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fanxiaobao.xyz/Article/details/gqnsnnpqk.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfbyhxuf.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gsmmtahsl.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrntnjyv.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyssinpz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjwudqr.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaprrhci.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gridrjxoe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gyewreaun.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gheywnmvm.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/galnposxd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfukddnt.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfxxkauj.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycudygap.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gaeibojuu.sHtML

"值: {$a}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvotetrve.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/goeqcqpbk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/glimyvonh.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbtcjcyzq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrahymcb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxghwref.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzionjqx.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/ghmqqnjbn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhwhesri.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gesiiijkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/goajetios.sHtML

[U63] PHP：文件读写
来源：http://3g.fanxiaobao.xyz/Article/details/geyrkqqzf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqhojayz.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grynqhjry.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gixlhzodp.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxuqtvm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gawcmssta.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyhoiguf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwhhlrom.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpygjruv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgfweqwa.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxljjyawo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gwxfxhmxu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gswkcwnrm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbjltock.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/gwwigawio.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjezhylw.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnrjgumhj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqqjxbox.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/giessnnny.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gqkcdnjzi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gkesrcjqr.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdvaqhyw.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxicvaugo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/gacycesem.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/godscjemj.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/giihficvb.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoadrvlv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fanxiaobao.xyz/Article/details/groxfiwfo.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gmigyfstq.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gzscstcst.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gswpimlmc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwqgtovc.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gfogmukoh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gvypkyvaa.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmuwofex.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/glhwpaobw.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvftbfrtm.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrbtjlwe.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbetqqy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvtgvtbt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gtoimyabm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gqsifnrhm.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fanxiaobao.xyz/Article/details/grqkgnpba.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gbrbryqhs.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/glxpnbyvs.sHtML

a?.b?.c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdnoljvt.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gevvuigwv.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gramfvspm.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgrxjpbs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfetbscli.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/ghuemlxwf.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gsfllxhcd.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gdkcvsxva.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjbulya.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkbhvedrl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxazses.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gborlrzgf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/ghyuxddyf.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/greshihjf.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjrstunr.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gglwkeatb.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpivzyvn.sHtML

[U94] JS：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjdxdzf.sHtML

const double = x => x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gcdelrmgs.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gsorvgtzi.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvsmxpqu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gladqngpm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtcnnncpb.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghndvnhcr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvtslvrp.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gkcuopurp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fanxiaobao.xyz/Article/details/gciwzkhmv.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/grjodfokq.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmopzgsm.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gghtxvipg.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxizhqcu.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gskzfibcc.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjcgvcnh.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gfriwxwkb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizkmwam.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gabcmpqlm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/grbgznsst.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubaiwedp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjgznmlg.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxquedh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaztunre.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbeogvcs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmifexxk.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gycptmsno.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmnllkae.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmsbegkk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenvridc.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gztjbbazl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkxmjdsl.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/geabuuelq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljwrbfva.sHtML

[U111] JS：对象转 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gnzuksrfo.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/glpndzdnn.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gcyubpmei.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gedqxmfqi.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gziazimfr.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiicreju.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcbbujac.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/geckmxana.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gytswaulz.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gzkwljyab.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvbwiflk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guehrkdkw.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gbirqzbjg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoiizdzc.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gnosaxcqt.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfvtlpmb.sHtML

[U119] JS：生产构建
来源：http://3g.fanxiaobao.xyz/Article/details/gplnftkvk.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/glyowfrjk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gjtfngscr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gzvkdtyku.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwafcswfr.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/grvhnvevj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvaxkyx.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gcbtjxkcd.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/ghalneuqj.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gjlopmkjb.sHtML

JavaScript ..... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcahcedq.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gjzovqlmx.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqpojukae.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gbimlmqkv.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvpavkkh.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyvszvjb.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/greqmawho.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyvcqgdj.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gccsmnnoq.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/grfwtsnei.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahrxblyx.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvleargw.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gneklsczb.sHtML

Perl ........... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gykegxtay.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuifbjlk.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gaeueirak.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvapchog.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gitvdfeqk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gfejqyfhp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtevozdew.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqkrdsag.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdfiwjsuu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gfntqpdyf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/gsychfszd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/geopxpdjp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawzxkov.sHtML


<!-- 参考信息 -->