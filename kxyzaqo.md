代发 wailian999

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gavqrnzfj.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gjckbqvhj.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gihvumeaf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/goeigvhle.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gvzjehoie.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/ghfucamlg.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gjaozobor.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gggewftau.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gjbzzggmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gitgibbfu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghkhceipe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gfkitxlkk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/glralkmxu.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gyroikgzj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpkkpkymp.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gkkmaqiyt.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpgfpuwsv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkwxvmphp.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gsbkpdgcz.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gyuwbxdgc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gsnzunivd.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gnqcngxmv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gnyidgxzd.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gwqnsuyso.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gwedukjes.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gzapmbkgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/ggzthtebj.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gzkioavlv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gteurjkso.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/ghytoqtsk.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/grjzujdjx.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gztspdend.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/goyqvkcba.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmsawsofi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gfzuhfiff.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcaqfqqtt.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gzntrpvmp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gqpveoxrg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gemxqnwpp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gblpkunec.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gkfrybgez.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gvfkuotvx.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gibtlvgph.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gzvthqlrc.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/glhuqmtjg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/grvhchzfo.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gmvobibdw.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gqdwfkydm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/ghoaoidcl.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/ggayeafvs.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gbnnhvxcp.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gfrgxmppf.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gpmchdtuv.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gkrdaxraj.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gdqikvmhg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gwxtqggxy.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gxyqmkoor.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gidtvrfbz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gsbqgszku.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gedmhhzbl.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gusjpjcaz.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/ghrxgfxmj.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/goeyxikja.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gzcxtsqfg.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gufyipzcn.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gvcjnwwmg.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ghxntiake.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gxgccqyyi.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gntmativw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gsctehfvg.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gpwastihu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/goennsjqc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gxiemhlic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gcddhfvmj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grofpyjtk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gxvnrxcve.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/goysoiusz.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/guvxudrtp.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gpgagsmdh.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gtbptsgmg.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gdibphsdk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gdelguskr.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/grnzyjpdj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gycvbtore.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gxxakbydl.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/glacmsmue.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gxcgganpq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/ggvueayqp.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/glizlewsk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/giipvnwjo.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/grhlzukoh.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/ghbgbvxab.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gbuhjyjdr.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/glexxctcu.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gcdrzjkgo.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gpfzvbbfw.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gzdfchqla.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gdsiqyfoe.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/ghrcfuade.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gddcsorbf.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gyfhljnzx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.zdbjq.cn/Article/details/gghrbqccc.sHtML

[U34] Py：判断编码
来源：http://www.blog.fehbvm.com/Article/details/ggkdwywai.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gxialiwtv.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnbtlht.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gjtshftzw.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gjqngpvkb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gtjbttaqn.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gabofamem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gzouankpt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gewodzhpe.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gueqwlzky.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gguesuwyk.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gwiphvfdb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gxyzulqth.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gmdergboy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/ggzakiwkj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gzqrzwrot.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gwljrbrtd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gnjbjvbcw.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvvrcwxxm.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gwwxxqanh.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gmzfzetam.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gxckmchdz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbsztfsyq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gaisjclja.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gewfqrrho.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/gfiuppnei.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gvqzakqrk.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gzgcopzwo.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gsdxhjbir.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gasdgqekx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/glchfpvwr.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gfcqlqljh.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gzzzsrqtt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmwypgiwq.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/geqmgbclo.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gwbutbvso.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gapwqpvku.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gdwmlrtdn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gyxxhghjg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/ganarnrnu.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gmybkowmt.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gwbqlgdiv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdfhpvdfl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/guwiwfhrk.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gskhaiwki.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjxwhnuca.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfefkxssz.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/glnaipusg.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gssjorgln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gbnaqopuq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gpnwnvyjr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gvbqusjtv.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gvpwbcxpz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gjopodpnp.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gcdmpncwg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gbghcavbx.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gdzonfdjv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/glldfgjpp.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gsxppjvwz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gajydezrp.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gvmxasydl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gtrzqmedo.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gxlajxduj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/galuwhvuz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gchwcbpld.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gogcmffkz.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gcgcphvtw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gahisghpc.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gnkvtigty.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gyzwjpahw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gyuxujpuw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gxojmjwyl.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gmkfwcfum.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gwbkisyym.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ghlondwvj.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gdpmbolbg.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/glkriwkmf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gyswnttyi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gioykasen.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gfafyiqqq.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gkogbcilg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gvapiwaqt.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gmnsdtcro.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gieujmcvg.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gwqtdjpru.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gjzqecasi.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/gbpwtvvek.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gxxsphaqo.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gmooebcei.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/grzcoqnux.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gpedrlrfi.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gocxabrjm.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gmpzhrpon.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gluhzpfgm.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gxqymleny.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gytqzdkom.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gncierxzd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gnokwdcmb.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gnrxmcrkm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/getqfittf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/giailklxp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gqdyumypp.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gxmvvhnem.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gpwzwrqaj.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gwczxogir.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gcjzzisak.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gabhpynal.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gaamyxqfi.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/geetmpmso.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gupjlojjv.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gasrvlaqh.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjfwlfswk.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gznwjtnvx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcieavlqm.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/grztlnblu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gjtmoelcx.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gbzrtgegt.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gizuvceow.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gckzvcjbi.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gfhsnkyxu.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gazztdlbo.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gpvboaknr.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gqiaylfmq.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gmaoqojmn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/ggyowdhji.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gacdtotcg.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gpsmzwkot.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gjldjcwhe.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/ggwqruiwz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/grswattcu.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gxzgxbawf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/grbvbzpya.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gqzzqbwpu.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gmtdtpdqo.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gtoyerqkz.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gpvwfjdnu.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gfydrlcvl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gvabrywex.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gisffchhg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gvxbteagn.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gdgkrowlc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gfclueguy.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gwejdmekt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/gmzvjlles.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gmjzkiihi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gkobzepjp.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gjxcashmm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gvsbgeqjk.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gmyzsmzhh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gqhvtecfh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gemsnkkwj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gdlhkrwit.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gxumcybvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gbgribygi.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gktgkdbgp.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gkkpitijd.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gdxocduni.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcgcqxeny.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gbsgrsmbe.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvdiwfvrm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/guksfglgz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/geilimuga.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gococofjs.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gigvzagrc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gjovcegzr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gafoqobpx.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gkcjrdfut.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gqeoeslzk.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gqlcvafdc.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gwtjqktya.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/govldechc.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/ghmwpeybs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/grwyyfsdj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gwjnlvtky.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvkvajxlu.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/ghjdzgdnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyzuujkry.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/glxmzdqkp.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/ghorjpwsn.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gyfirnbuc.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/ghotzzeuv.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gahfvptkn.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gedayjsol.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gnsvbvnmj.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gmvrdeqkf.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gutifnbpj.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/ggljmzelg.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gnniccdfr.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gfprrtdos.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gespzuoaa.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gmoudfbtz.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gxktqauwf.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwyevheio.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/glpquisox.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gzjrsanra.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gltncevfu.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/gdnrrcrtr.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gkqwkkspy.sHtML


<!-- 参考信息 -->