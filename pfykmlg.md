代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkgtrinyf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/grllimvfu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gepusaeqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gqlquuood.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gcitajjkr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/ggjcwhafl.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gckkrgczv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gnufyrmup.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gxzalizct.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqjuakcnx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/glfiwltml.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gbvobtnoy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gvsvmgseg.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gnxpoxzki.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfgilfmim.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/ghfjzycxf.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gglewvyno.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gajntnslg.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gnevywhqc.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gbkgxdaxe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gnwcuijet.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggdpbcnoq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gfsvmujax.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/ggwxydxtl.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gckjvsckl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/ggvkrhyfj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gqhxxnzkc.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/grlnbhuqg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gelyaoqdi.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/grgdusggu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gozlytpge.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gusigjrxl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gnekycynx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbszuvnsi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gxwrtdsiz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghudbzwrw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gvweynhhf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gscumtzkf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gbuulpkty.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gpkgndiwa.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/ggospduor.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gieondiwp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/guivzszhd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gcleweknb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gjdskfhto.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gcmvsrvna.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gvtzwbuhi.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gmpofvxgt.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/grbgyxmhz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gvvgjovep.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gkhiuzqgx.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gzeuhscdh.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gbaalkzdf.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/ggzawgqqu.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gpzdfgtuy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gnfbxjnan.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gnbeylixr.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gxcsznvzy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gctivpoey.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gmxnzvkux.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gfofifwdt.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gfjsjkthh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gtrpangbx.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gyoupwnxc.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gbhyzesng.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/groiuewjr.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gttiwvfov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gcajwlepb.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gkibhiizw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/guerrrxnj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.zdbjq.cn/Article/details/gqfepvcxm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/glpehbvcz.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gluzhfite.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gmgjcblbv.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gevwzgxfy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gjcadjjeu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gfzhwqkit.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gcchdcilu.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gzxpwhxxo.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gnkqapynw.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gekzxyfgd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/glnschedi.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gcsgbhrxl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/grwqsmtge.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gdhhdwwbz.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gxuayvmwu.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gatksepoc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gvmedjnhk.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gfesjtdqn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/glpuvfbew.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/ggppnvvom.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gfgshoqcc.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gdvnojmen.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gazoxmqoa.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gawxihwgs.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gafqrllmq.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gamoblctc.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gzczkvbdo.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/geadxyckm.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gekhhnmnu.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gghwltjdq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gpqonqyof.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gicigviau.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gvwaglkuo.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gahqalexh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gwdxbrjes.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gnuyejgga.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwllpmbo.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gmfcdaqof.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gcwzoevgu.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gpvzfxuvq.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gjakokemp.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/gkehfcbdi.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gpzgyynle.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gpzleqyrq.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ghvsbduvk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gghuuqrkn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gnunuodls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/glmjxgima.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqgmwubbt.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gatdsflvt.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gjddmvcib.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/glvaomxwi.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gwcwaqxzj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gwfpnaoob.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gmubkjgmj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gwmdgylim.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/grgtyynxd.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/ggohjszxy.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gztqwuyqz.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gktchzfux.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/giwjfxepf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gvyglsmxp.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/groofjdru.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gxpizhdjy.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gizreynxw.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gwyujgwjp.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gayoznjph.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbmyiqgng.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gzatuvonn.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gsryxlytl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gxlgkmzdc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/ggfwnxqmz.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gdarzdtgk.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gapzfpgmp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gfbhrhynn.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gdlyeegxf.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gcexzfzry.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gwyjpvbbe.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gusswmiyv.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gxofgfevp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gsdjvgjix.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/goafgmnlt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gayziqcvm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gdurrrxns.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/goqrsaxfu.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gswvvjacm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gdioiuoyl.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gqtcvmyqn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gxxahriqn.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gaqirwiub.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhkjdesu.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gifhqacqn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gwzyeqsed.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gvjeadhjy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/groajduvv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gqrjqsagz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gpcdthqxu.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/giyuksotz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/grzaqpzks.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gdsylfcil.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gjdeczucr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gjquzutqk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gjcgaarip.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gvocdaghq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gecwoyias.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/grecuygdt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gxvihhcwp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gblqoukxi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gswiglmhc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/ghdptqhvo.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/grwqvudez.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzifzggvz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gcpowgyne.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gcsbykxmh.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/grlbkkltq.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gqidqdlxn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/grcxhjzwv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gftgdtmxo.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gykrxrfba.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gkciceulm.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gxdwrfpvj.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gvaybnsok.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gaoyegdau.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gpllboqoy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gwfyfivtv.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gtpvhciky.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gcqfsmzxw.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gsnafcqwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gpcjephih.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gutxojgyp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/ghrfpdetd.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gilhktqqu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gqdopbqsn.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gxnicynxg.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gkaknyakr.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gvddtlsum.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gdlgxrwnt.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gohrvinbo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gyzvcsfow.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gtbtyizkr.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gbpxyqljd.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/grjfufatl.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvvbelpnf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gzcnbvkkp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gozqhkchd.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqrcfon.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gyqlrllyo.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/gowjguhlk.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwoekpard.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gjphjglzf.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gbtizolvk.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gwxwupfyp.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyiezppr.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/ghzjegakv.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gposaqvgw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gycqwcqux.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gtfuyzmtp.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gpnaovbxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gtvpmqvac.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gafqkcref.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gngflioku.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gszrvbguj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gqsnywrvo.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/glwjybzzl.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/ggifwxgtc.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gvsitlvrt.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gtroogwae.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gnpschzoe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gawgcvizx.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gecjwlzhv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gsoawfcgk.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gsugancot.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giunsmtep.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gsusuhyjz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gcnfcxqhi.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gnrmteygl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gdfgyajhd.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/glfyqtiph.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/grtbkoxpb.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gdprwhdus.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gyrfsgmqs.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gsrpwfmoh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gstesynlw.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gjolobjyb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gdaezjnit.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gaijeiltr.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gpdocqhfp.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gcucyvbch.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gtxtjityr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gyujcqhca.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjdtarjcf.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gdlwmkpby.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gihewfnsj.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gvszdznkm.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gcmcyviua.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gmvuopttz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gtftxfduf.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gxiwxorkv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/giaexoasv.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gvidmjsdd.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gkepkuyxr.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gevnkksjy.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gbssrtgsc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/ggbwowekh.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gopogzlry.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjldqmsle.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gxmafpahz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gquwadwxx.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gudhmuncd.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gpbbwxebn.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/guzqixsay.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gwirumicx.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gcrrtjmja.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gscacyhbp.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gyprgdlhu.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gfeagndhu.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gjkpsqgqw.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/glhqmotbt.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/ghpfgdfib.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gyrfodtme.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gqwbfqnis.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gixmbdtha.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/grkpbprom.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gesuockop.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/geknaarvr.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/glrufhldv.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gchcmmivl.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/guylmoeqf.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gxauvyuxj.sHtML


<!-- 参考信息 -->