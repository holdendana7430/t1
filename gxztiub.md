代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gzgjjbliu.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gaefbbfod.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gekcnstnz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gncsvfwgy.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/geggmlyqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/ghbbuvvza.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gukgjjmuj.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/glhgrgtml.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gxqmtffga.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gsbrdfsba.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ghbtbiyxs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/ggzmyxcbv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gzlwfzwpb.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gootkpfsl.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gmyqthbza.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gvtvowtjq.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gihebqead.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gojlwjyfb.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/glctwlzvh.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gfdztbpqv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gnnrphfvv.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ghpvuxmbu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gmgnddoso.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/ggggfreev.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gkweuqqrp.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gkbxegsku.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/geemycxbz.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gaawswhbr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gvsweejxt.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/glfxdjwna.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gkdhshqxv.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gvdebhxkz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gcelyfpwe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guglzzzha.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gzilorarj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdwzqgenc.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gyayfiykg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gfvnpqist.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gjgomirgh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gdkjgigxy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gknzagqjx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gnsclbbgz.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gcvokkwte.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/geuqwgzms.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gavbizscu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ggwmkbkwr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gviilfuuv.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gwyigifxg.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gzzatztuq.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gsgxvtoqv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gmlpeqzzq.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gbxyiceht.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gjyfgbbug.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gxbazzojt.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gjhmydfcq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gzcwyhkdr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gpdklkxop.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/ggmhjhhzd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/grxydovma.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gfpztofhs.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gydpzyszv.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gibtygmdt.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gtffywknt.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gjiwftkde.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gistbsota.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gfdccwqwb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gtvkpgcjb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gfoekpkdj.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gahslazca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gywlnpkoh.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/glibjchgh.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gnduufzgd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gawbhfiyu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/goubjbsos.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gdktbtmtx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gchazqyar.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gfmftrhyh.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gqwojjbke.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gwzobxfdd.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gthyjfmfu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gnhucaxra.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gikfedrce.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gjhapwfjp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gggybcuju.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/grjnvievn.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gwosxeonx.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gkbnjdtys.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gaogggxzh.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gmteetzsz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gmsylkxyi.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gghbgykfx.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gnmbmldfl.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gdkthhqmw.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gbzdhxuju.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gbterfmro.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gijxuvhce.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gahdwyzdl.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gskiqiumo.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/glvkigvuc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gixocuehs.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gjaarmokj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.hesvh.cn/Article/details/gxvgehrwj.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/guvgmaqdw.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gwlekhvgb.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gmpbcrkxz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gaceimoow.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gbquwejko.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gobxyistv.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gggtmkomg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gxvjuzapw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/giarqqmoy.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/guubioori.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gyhiceudt.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/ggkkhixhz.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/glhvdufkg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gyjzxzbmn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gxmojwijy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gepjtpmnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gklkijqcj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gjvdxpfzh.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gzsntdfyu.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/guuasdseq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gajewhweh.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gteukiqdg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gwtcdnfvi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwtwubtuo.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gqngqudgo.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gsuzcewyn.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gykmxcmes.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gbumoomxg.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvjbggskc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gafacgvei.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gubvyygqw.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gfhlmbazv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gsfjfixkg.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gcaujxmgq.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gxhioeygp.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gymkaltem.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/googymhgx.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/glubzsqmt.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gtwxferpt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gvburwfpp.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gqyrvfabs.sHtML

$obj?->method()
来源：http://www.share.hesvh.cn/Article/details/gqrursigy.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghywugtqx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gnoduuogx.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gfeadrnpv.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gcrfonhys.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gewugrqbk.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gnnvxyqmq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/grlydmpln.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gosxcsiau.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gwdkfgmsd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/glvwadors.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gepscikcx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gkbqngwrd.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gsbrxlarl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gyszpkhoh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gcsmlmdvw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/ghkhwprmn.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gzcirxjcf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gadhqovht.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gcehcrhre.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gjncayddn.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/glrumaghj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnquiqnei.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/ghhwwchsa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gnvigsyay.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gorcsyxep.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gpqewmsez.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gtqgjmxdo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/glfwoypfs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/glytevfcp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwvljhriz.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gfuesmmxw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gbhjkvlst.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gzdgdfctl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gluhtknug.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gxupxzbuf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gxtvonifd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqzxddc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gwqrforiv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gzheqpkgr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gbmdhdzum.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gcfnxrfxo.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/ghroykggm.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/grczodzzf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gpnfyakxp.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/gvlqwmxue.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/goddgixjm.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gzptjxvaj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gejdbzuro.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gtzxxzfcz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gkbyghljz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gpfzjsuah.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.zdbjq.cn/Article/details/gbkvrhgel.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gmvvpwnsc.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gghmpjxnj.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gszojbudr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gpnlkdjpa.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/ghgvdcgaj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gmiywiwzv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gquonprom.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gltpaawxz.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gbscxrngh.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/ghifjlxkf.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gfohuokfp.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gljldksed.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/ggzlxgzwq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gtovvbodr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gktnqqygy.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gdfpykxht.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gdsltamxc.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gcczrmnhq.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gknmdmyad.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gbuhxcyhu.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gysjdcdjg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gcziioopy.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwwufvehc.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gucztuxnx.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gsscbskot.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gtzknqgzg.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/ggqwhdxis.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/glqsigopr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/ggeuxqwye.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gepucdark.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/ggcgjulla.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gcimmlupe.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gbdldjqtr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gdjfkpgac.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gozmytzgd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/ggmslvnwf.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gtwozkouf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gujuehdjr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gckktnkuz.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/ggyabyrih.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gvlzuvtup.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gbzlneuti.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gvyvsqnse.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gckgyyjql.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gfshbbflk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gjqzkksyf.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gflszbmry.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gomdizdza.sHtML

[U105] JS：节流
来源：http://read.share.hesvh.cn/Article/details/ggwnatcbl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gkivmrkre.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/goaatfxig.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkjzltp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gapdelaon.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbrjtldxp.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gmffjaowd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gxpboozgv.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gwxhihvbl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grjflqavh.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gojdwuxuu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gmslkeyhl.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gcqgypiom.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/grvpevycm.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gfmvieswm.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ghsumpdol.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gcxhpejrw.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gazshvlsl.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.zdbjq.cn/Article/details/gwtxxtcav.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gyswlmhzm.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gmajiofuy.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnmyytjak.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gnddpbtzy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gdmlzfgrg.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/glcjanqcb.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gcwobsptw.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gxufdmxjk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gyerynnnu.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gfnlyasqu.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gkigxccxh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxnbofi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gtrfbvyfl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giooymqvh.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gnfycxehe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gttbjmtes.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gdyygggpc.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gudogdgsm.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gyxgqafpo.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gxfxpggtf.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gmhjtjzcp.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gejuzvkxg.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gdkpifpgn.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gjlbockzl.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/ggmfxggfn.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gzlieziui.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/ggsqimbat.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gsodbubye.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gwwqddtrl.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gvyivnbrd.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gswusgfck.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/garxeuzqi.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqxqvxo.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gcgkuibth.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/glloeqfyb.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gwjlziuub.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/guilmzwha.sHtML


<!-- 参考信息 -->