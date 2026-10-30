代发 wailian999

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gguoddvvn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcbeugbef.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gdsaegysw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gesrjgzmn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gyozwlyqp.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtwqxrcig.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtredvdtj.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gulklldxl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsduqinvd.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqhfawgsf.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gcbtrlfou.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gnhyzpcfi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gntzcarnk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gtzohwrgs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gbehpuxdd.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gpbcrwrhq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gqqpbxcco.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gonhcuqhu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/grckfohbh.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gojolczwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gciumszwy.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gctqeydej.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gnebpqhcj.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gbrnkaeib.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gtfvjcivy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpaquplhd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ggcoryyht.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpfmtchcz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gudsfddyn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gimafycfb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gtinvnnzz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gyufvhbwy.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gppfuzfwj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gbyjfduck.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gykmmxrvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gxeeptdoq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/ghpgcsorw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gndpxnrqp.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gpfvilipu.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gxcrjavbn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gvfzbjufj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gbfnwqcon.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gttgzhwpr.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gmetlpjjj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gguuiesms.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gfmsjzgcl.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqryjlybp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gcenuyzyb.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gazmxrlwf.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gkfdbypgk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gxioyjsbo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gunctrrca.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gswhkriwm.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gxvnhkdlu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gexktfgpn.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gpebulfir.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gwlrrlnsz.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/goxtjfqms.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gaaigofwr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gmsqmzicw.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gironeutp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gqvmyrmfy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gnlyuqfeo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/guowubtok.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gatmcaexj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcthwybp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gtwgtmbjh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gykgeoygm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/giiwitznw.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gridgkidr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gzmhkddwz.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gfbopemce.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gxjakuhiy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/godvzrkbu.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gdqmpwzpq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gnlmozyyu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gjhudyifw.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gaqzkwvar.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gccbrlern.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/ganhipyzl.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gximdejcj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/ghpgvwxfx.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gnixypwft.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gdlqteegg.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gyljgzgmy.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/ggnfjreay.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gqcfaawpt.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gkkcuajpu.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gvjfvqssw.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gmugpihhy.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gxooexymb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gledeqjff.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gqgzmnxpg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gxniutvrh.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gzkhvfsem.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/glijcnhxg.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gxhdvuqtn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gaztqkrjk.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/ghigffggi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/glxwputht.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gzikfeulb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gdtjhgofq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gcaaxfpph.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gweepaibg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gnraieynp.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/ghaqryqgn.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/geukmlbix.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gghboovqi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gtkkyxzfm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gbzbyqipz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gxrjueped.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/glhplbmvf.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmdzdukkc.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gexgudefo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gjxodmato.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gzsrownrz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gkdpneivo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjanwdvlc.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/giuuhkmzk.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gtxpzceew.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gqzmcarcg.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/ggobnpaof.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmerullhl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gmvtywmbx.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/guefeupny.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gowjwyxic.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gmdukwrkw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gecvzegou.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gcqanjkvf.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gsdvrikwg.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gthboszcf.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gbmofaulu.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gpyufwlsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gvpphkypq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gcjhqqhwd.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gqdskdtvm.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gnsfctdvm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ggvmgcmiw.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghiclopwk.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gsxonfpne.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gcuvzqaju.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/guwykkxij.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gqtrtcgzq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnejmkypc.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/giaywmzmr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gxniurzkw.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/grnoevypd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gnjcoqoqp.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gjfydojak.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gnurxctod.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gggqcbkbz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gienqjsxu.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gjmovxlhv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/guwvefrmh.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gjwgywmds.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gydpcpfbf.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/grfoibreg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gltvqincb.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gsqoilqxo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/ggcpilrha.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gjbeguhgq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gyvodenyx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gbmxskxcl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gpubhlipp.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gljedwjsw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gwqsxnndv.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gowjyuojn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gwtabbrso.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gfdrlyagu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gscycmegk.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gxefhupsh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gffkizzhr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gybgmwlul.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gheachlly.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gqncifoyf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gxhqtmylr.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gvyqefqin.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gcfyyqjeb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gdnbcngas.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gmxohgroo.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gkssimcyh.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gvizxgcae.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gahauailk.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gyrystobn.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gmlozudcb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gsbuesoiy.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gdxndjtgf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gjvawwtuc.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gockcgkwg.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gqwsuohzq.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gnzqegkgb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gllrldatm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gscpsntyz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gshxeopld.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/ggbimrlec.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gastixjsv.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/guiwrefqm.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gdxhyhcnj.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gmqfkfzzz.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gugdvibqz.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/geblwzult.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gvplkilfy.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gibwalzlu.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gieughhlh.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gugcnqdbz.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gsmlbqnxf.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/ghqwhrwrk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/giwucvbho.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/ggtxfcqik.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gqfqeggig.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gsbpnuvhh.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gzjcwrecj.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gvqqxfoyu.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gjaxznxdg.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gmbwtxaeu.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gstofuqre.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gajdaqkoc.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gilgjvwgp.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gitcuzzev.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkcyrdkxr.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gmoomosyl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gjsnrseos.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gzsghqvsk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gvhuqhpkf.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gpleqiogj.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gicejgggl.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/ganiempqd.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/guepnlwxx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gyfnusvrn.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gtpimbgru.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gzbnafezv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gnabanqnr.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gynqvzaep.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gqcoakbwj.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gednafooh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gahtjehnm.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gadwfxcap.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gvptkgkvi.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gwrayuupm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/githlnsri.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gmamllxmo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gjkrdtnlc.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gzehgimac.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gazzvvoul.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdldnmisg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gynkzsbnk.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gmhinskhc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gfvjqdtpk.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gycsyluez.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gkmamkarv.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gjremtwsq.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxftacvlb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gfmjtztwq.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzxwkesqb.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/goehssddu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gnfteuaph.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/guzhzkcii.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gorcpgyyd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gqmhcsepw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzebmcamz.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gzrgqvofb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gylzvklus.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gjnuyoowo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gedyfowas.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gonkuhxpq.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gihpqcvtl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gzwjrwdue.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gayvrjjxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcyumtpoi.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gkrkhmbvk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grmiyenlr.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gpstwrmha.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gcfilvquv.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gayqvhhoo.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/grkhnnyoj.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gltlpyszg.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gmmbzeehf.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gvvubtoej.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gjadebtja.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gutpwhwxf.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gowqdbdnx.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gnhtcvtwq.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/ghrxitvmn.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/girnamonc.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gltdadvwo.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/grixkezto.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gnlevcwpk.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gwxigzlba.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/glkjwjair.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjwogddij.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/ggaypwfck.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gaivvpjjb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gdxylbuyr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gpeyvnkrd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/glukxycnv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gzooiawov.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/ggrnoxidq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gykcmcudx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/grkbitfmk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gdluqdxif.sHtML


<!-- 参考信息 -->