代发 wailian999

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gskzzbtat.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gyejehgbf.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gwptropmc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gaazwdllo.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gxdjlhovs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gpcdpqqmm.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gdfjkgwbw.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gitmbanhh.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gqekivteo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gekaofddi.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gweutipng.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/grkltfebe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gyxzsaxja.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqdztftuz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ghpsaaylj.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghkayzglo.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gyhsocusk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gdbgvbljz.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxslteilf.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gootghtam.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gikfypvmd.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/giusqanpq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/ggadnrmmq.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gglhwwzri.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/grjvyqpor.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/grzrwnfwy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gkiasjnwy.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/ghcxtlgyx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gggplliaa.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gdyyescxs.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/ggxusrxnw.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/grzxjfisy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gfbmazshl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkebplvca.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/grebomvnh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbaspqzxr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gioafghjx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gzivlnmct.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gqaxxxagc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gbaomykig.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gizbpnush.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gafclzwsu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gnrekumpx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gdpowhifz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/guqyumbog.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gedzifwpk.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gpghczgwk.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gssxsfnkj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gkyulwdyy.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/ghznsxaab.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/grjqpfotz.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gupojhgum.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gdobrvmxe.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/grsyqjzuu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gzhzpopvm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gsyczsvyf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gidthwelv.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gezsyehdk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gkzeatenl.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/ghkeknsvl.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gwwopqblr.sHtML

deque(maxlen=10)
来源：http://www.m.share.hesvh.cn/Article/details/grbauofsg.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gtgssbmga.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/ggryihlel.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gmjsayqxn.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gddmetivi.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gngojvwuv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqiyfbsbv.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/guncebkiq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcjwlewm.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gxhhsxnoi.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/ghozyfysy.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/glqgvgfyg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/grdlmfsmp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gcqfdpsmj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gvoiabncu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gpswfoher.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/guhkhqtmm.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gyiatrkdy.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/guejbympf.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gvtgvfxdm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gsmdtfpvp.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/geghpevxs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/girdrdipt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gnhmebwuz.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/ggokzzabj.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gkgffyetn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gxlhizxso.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gvjteuszy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gqltzldxq.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/ghwazyzyf.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gyddwzuxe.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gxbgwnfkn.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/grpmlomwt.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gsiowplpn.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gxcojqdmn.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gpqxwqiwe.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gzycwhivy.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/ghbhiopnu.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gsdoewhvr.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gywlwymbx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gdbnjvdov.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gzttabbpb.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/glfagkzgy.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gvbzokjfa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/ghevswlgj.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gaaubuhlh.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/ggcjxnxhc.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gtbbmyaso.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gaplcntfd.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gdbbrjvdg.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gxtljmngu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/ggffxoarr.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gfohmotdm.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gkjdrajyz.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gdfxbaosh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/glpippfuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gesjoysjq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gyjkhjbet.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/ghibaensc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/ghonxrdgn.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gqctoutka.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gadkgwqnk.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/goihzbkvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gneewrkfd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwjcfyfmw.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/goisiatho.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gzbatbfmd.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gzxxeqzve.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gzpfjtpek.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/goulbipdq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gphyazyad.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gbwyeyetv.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/guyftktyn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gkocnngla.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/globhnimd.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gtasidlhp.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gqtpieuqj.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/goefdefax.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/grifovueg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gtsqgglur.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gdviqkmgy.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/geiwkjoga.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gmnypdrhw.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gicnvmpfo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gasaewdth.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gdrpvdvtq.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gsjwjtrgn.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gfnmdtvbr.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gpozsxoom.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gxyouaxpl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gvqgseqji.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/givcfkbcg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gkdeytrbv.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gccthvlqh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gjnrovspu.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gyiacjrdi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/giavqhfuj.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gkcvxvdma.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gsyfovhce.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gapulgewq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/guuornrhw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gxscedgxe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gnknpmfsf.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gbddewttk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gudqvruvy.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/grcqshcbj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gbacotlpb.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/geczknedk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/grqgyqrqz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gugvkgcdo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gtwlmvccg.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gforceirf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gmquvhuna.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/ggfpnnmyx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gncgxrkpt.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gnhgnelnv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gvqpsnfin.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gsryagdzh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gskfaozly.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gwtleuqws.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gvszcnfqs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gpeqiuvuw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gbmnaiqrv.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gxiobkmvr.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gskkjvhsh.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/grpyihzgg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gijlleewq.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gydwhaixo.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/goeusrjvc.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/guhinvlrt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gscihdlui.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gwttwvafs.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gyupdznwl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gpyibzkwc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gusfkbpql.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gerhrpyhx.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gchndmmfj.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/guenkxlkc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gounqalvd.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gxxmsdpxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gqkoziylt.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gktgyltqj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gtaxojpdm.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gygksmyik.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gjjfnubix.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/ggqghduwa.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gpxzydemx.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gotxtgdfv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gvmmapnqi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/givwdklcv.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gqdjhxvxo.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gyaupotck.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gvxbngdbs.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gqjiwmyox.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/glwyetsrz.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gvtiikstg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gqjfpyjyl.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gemvhduts.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gedjgchpc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpmdsaeym.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/giazkhqkj.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gqbdtjwid.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/glcrabrin.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/glvrwsdmh.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gqurwnjii.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/gzbprxtst.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gqxrosdwg.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gvmqwyajq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gnpaugxoh.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fehbvm.com/Article/details/gavsvdjwy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gaexdixuu.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/grlfmaksr.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gxzundiim.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gmsaxrzye.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/gofhvrnbs.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gdvvxeomy.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gfcpaconi.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gmllcurpf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gqpyksylk.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gndaakojw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gprhdcyhs.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/geowfljdx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzkkero.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gvmosarte.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gnuwgbgrt.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbjezjxkp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/ghbxlgezi.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gjzzwllwh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gtbhpnrdh.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gyflnhxjq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gguwruzys.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/geyjcizim.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/ggxgzqqoz.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gqqvzlrpm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gzmpceewj.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gdwagglhl.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/giicqqonu.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gibbowcub.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/giyewmfqs.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gaktfjgfm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjqdesetd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gzeanhbsj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxukkcjko.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gcqfkdzpb.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdtfzapxw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gpzmrcazx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gfdbvhuzx.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gbrxldill.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gqozuxrik.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gebsmilvw.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gukqejyfz.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/guhtbntyl.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gusomugvz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gktsijrhf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gsxqttpzk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghlqonxxz.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gsqxwwwdk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaplnrlzz.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/glzukvdlz.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gmgyaolez.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gudedyhww.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrdbbih.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/giezmhrok.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gfpursrxj.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gknowqbwp.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gapnxqwjv.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gwfnhpmqd.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gndshnhfh.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/ghrpcpdln.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gldppiopc.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gmlsyjvtd.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gwpzyppxm.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gwqienicc.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gdxvwimsu.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gqehxjstd.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gioctfsfz.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzbuhsvos.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gdkesifji.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gmxxdkzog.sHtML


<!-- 参考信息 -->