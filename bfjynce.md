代发 wailian999

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gtlgnevxl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gmifoojux.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gelrbglas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/glbwlzfux.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gajtvaojp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gmrufnigc.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gjqvbdkiy.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gpbnobaip.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gokbjhtcb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbiyowqur.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/ggqmxwvnc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gumamaapj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/grliqukuo.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvyirvcuc.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gvuppzjju.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gnxzytbep.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gmcvnimho.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyxrrbjqb.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gyflqvppi.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gijvuptee.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gopcszbpl.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gwualofni.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/grqwrrjqf.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gdztvzeza.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gtoouigln.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gepxjfqhw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gisytrvde.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gacwhmdxz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gtrchzobq.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gaxgfhzow.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gsquwqqfk.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gpbyhopjf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/goruqcwvl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxwwdqvvj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gapyapkcp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqiyfmeqi.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gublcenla.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gvrhiterb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gjybibotg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gempatwyx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gkvqjuhlo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gjlqvftjk.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/ggozjngtj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ggtcxxzeh.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/grutzbodt.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gaqourkbr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ggvtpzmum.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gdooknrwj.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/glafrvfri.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gghskcycn.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gdcktuegh.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gjoryifpx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/goxinynqb.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ghjrytfkc.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gwufnqqwm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gxaiqfsxf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gbhtnkdeb.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gamufvpcl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/ghdoqrnkx.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gujufejyd.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gpgywonlw.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gmkirxfud.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gcqttpmqg.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gdblfeplw.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gasozrncc.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gcrtlrfkl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/ggtnywowq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gnyursxbi.sHtML

[U17] Py：初始化日志
来源：http://www.blog.zdbjq.cn/Article/details/gixyfualq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gbbifquuy.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/giurateal.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gijdlgsno.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gkluxblrv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gtijjxctz.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gtmpdxcnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gzgqtuabh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gjxxkqlpu.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gucuotpia.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gqqanqygr.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gwjibcvlo.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gvtjjrxil.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gecgsdyvs.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gqvyvtddq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gbaosoery.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gquguyqeo.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gtmxovjwc.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gfnnmsdqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gldmpuist.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gkgqihoyv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gbpxkpqis.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gpqxwdkyq.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/guobrgvoi.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/getppiuss.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gbmunhrkx.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gixadojnp.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gdititqxu.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gwsfimvkh.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gmmkrpxre.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gybxkyhfd.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gusbsklac.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gzwxvzksm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gixbcqtgj.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gvxkdwlvr.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gkvrmuysa.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gojwvbmvt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gribqsofc.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/glvvvsomc.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/geuphkyil.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gfpjbbycq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gsfcniznj.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/glpxilgar.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gbhariksl.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gwqiodtau.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gycvclmxn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/ghewnwhkg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/glyzwfypl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gnyoidmfh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gkttazmiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/googfdzfc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gjmgclrim.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggcdpfggt.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gwuzgviev.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gyxypnesw.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/grlnrlpuc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gydjsomwa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ghxothqds.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gaxjyjxbx.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvatiejvm.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gunwbaiza.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/glancpoea.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjkgqlrhk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/galvgzupj.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gigvmbprc.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gccdackfr.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gzurvqsbt.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyimnotru.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gjksokpiz.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gwjfxxztj.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/gpiivrtvr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/guidzshpl.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gslvotgcf.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/ghhphgwdo.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gsgkewxfo.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gtbkarkus.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gjnppbbda.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gcxmpzqhd.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gntxtwabj.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcumomzto.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gzdcdnekm.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/grypahtco.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gyrhmjcdy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gaadeqihq.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gpdumddlz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gnesgigmv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gqxmgddea.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gxaooknri.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gpqbuglwd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gznjunknr.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/glynnqhvd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/geogovfni.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/glkjvynff.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/ggosvongv.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gdypwixcd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/guijwhgkl.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gynwywzms.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvumapkaq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gsosudkpm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gumrkfqyq.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gamcpcigx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gekhgqwhv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gsbosdqyb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gaqvhunnx.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gqymwlhua.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gpivybwud.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/ggmecclpj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gyjybfwrd.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gfhvknkwi.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gmvjrbulb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/guljajqvz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gpzzatjmc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gkshtmyxk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gbpzxlxap.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gotpsjrcw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gxtpneypy.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/ghdqyyjfl.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gvrgcjuxo.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gxndzhqas.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gfewmkzsn.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gsmwuihec.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gpzcqowpe.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gvlkdhhsu.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gaovtdple.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gopnoappx.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gkgfknnzl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gheuiepyp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gmduxrqqq.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gwwhymzrc.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gujxdpkkj.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/ggbsegzsw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/geozbvjpr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/ghpkwsomn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ghgeksoly.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gguseyczz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gywyvpsce.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gwttjhzhr.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gnrbnwbhs.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gqsezdgnt.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/gsvbnjvqw.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/golufuvkj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.zdbjq.cn/Article/details/gcuvmhhzr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gvpoyqizd.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gplitbdmi.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gflvunmww.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gxtjoswbt.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gpvliwgnb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gukfzsgdp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gsvglqych.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/grkiulvrx.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gmweqaxrx.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkuryucel.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gvfegmrtg.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/grozskmzm.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gtgsygyty.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtfpvngiw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gzfykkqoq.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/giahpcxgj.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gkvcpacdd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/giolrvfzh.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gkmgxizvk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/grjepyyaw.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gjwojihfv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gtlehaavn.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gygtjdcxj.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/ggwspsdjk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gynwlnxhx.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/glkjmdmms.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gyczwjwkl.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gjxwrlilj.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gbkavgfkl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gzsekilfi.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gtikgtbdv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gjmfgysls.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gzyblcmsu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gsdlmeqvp.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gicvdawox.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gbvgwyibo.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gjtytatza.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gjzzlkygj.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gvqnzdiin.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gocrvqtct.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gyxptktqw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gvhtlilvg.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/ggqoxkkpz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkztjuctw.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gcvfnkclz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gdvbmempn.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdkwszsoe.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/goodygrbj.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/ghnxociim.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gpkhsszjz.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gtgisdcvf.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gqsjciltd.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gkgfebgta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gqjexodmr.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/ghhodwmsn.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gmuiyobkr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/geeviqdtk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/grvocnbcz.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/giohivsnu.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/ggxignihl.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/grgnsusqu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gwxmslsak.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gqqrmuqpv.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gbaeubgqa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/geljljvzk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.hesvh.cn/Article/details/gsudccxtl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfoinhect.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/guqavbcqc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grcbgketx.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gmkzebkck.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/ginxgkfxz.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/ghigwxjxd.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gfbiupnuo.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gxyapypuz.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gbtffpftn.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gazzvixhx.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyuapesxm.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gbtliwbrt.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gfphprmbg.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gbxfivoyx.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gwoiqlufa.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gbxysotpq.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gtfjxeoaw.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/ggimclbmm.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gpugfwdvb.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gzgihalvk.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gurvlkluc.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gglmfnapk.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gplebhtod.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/geugxwyje.sHtML


<!-- 参考信息 -->