代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/ghkvqdzky.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/goobjzqlj.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gwjagtsba.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gbybwnpiy.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gmjgseayq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gxqzhpxgi.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ggoagrprj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gtnsmoceu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gbouysmza.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gegkcsrcm.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gomyusjew.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gmhnirqzc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gofldzevp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gvhxdusth.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/ghppmtsgv.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gvyhfajcg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gttcaisym.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gxbnmihrj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gltoksdmi.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gfqnbkvkv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gfozcitsd.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gqstffjba.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gqewutgro.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gfoewqqbk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gnikupbgn.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gwqtqyrrs.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gbjexbgvv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/glsfbpyla.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gyllnpgzk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzgkvsytm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gmizqacvx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzlhpaupf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/ggwbnqrhe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/guvuxbxio.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/guqrgzcwp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gpxntadet.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gktdhduse.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gdyzmihuk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gueappufv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gwlofsigg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gnplvjylr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gqktzeeer.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gxmpykumc.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gqdobkjdj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gzpwffpbk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gwsdvzjlk.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gdxjryasm.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/ghmiajlcs.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gsonphwdf.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/goavxwqkk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gmquryhny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gjpqmbfby.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gculnwyha.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gjgcmedps.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gzzcyfpvn.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gzhiisjaw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gquldqjrl.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gxtdfjqom.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ghhpnkqii.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gqbeflqoz.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gxmqsrcjx.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/grvglaajr.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gxfvcpklq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gbtoqxhjh.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gtluiczvr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gukcgqqju.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gbyxwmext.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gpwgyfmfw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/guumkrgvb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/guahnemyd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gbntruoga.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gfqvkialc.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gwpskvejl.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gogoiwjkv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gikgunpfd.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/gmvweqnld.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gtpaqznpf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gzdyktnib.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gdktzukpx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gwnkrdrjl.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gnhrflfvl.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/glpjtvklw.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gdnjcqlnc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gybppouiq.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/geqqjshpr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gidxystse.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gfvitlaes.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gdrpvnwrh.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gnkrrkekb.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gewkeyclz.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gqvsuhsuh.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gayiygbwt.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/ggxnbozxr.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gplstruhb.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gzwgoycbm.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gjsakkysv.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gpfvrgzrs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ghpfqrdml.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gxfdmocgs.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/gmlyzbtdx.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gfhrentry.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gazjfocgz.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gnfgywmvw.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gvmnkohcg.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gwbukxcme.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gtxhvuxvc.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gtahduyzc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/glmtfbbai.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gyhecyyuy.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gjomxqsvx.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gsarmevex.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gkbpziubs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gewxamyge.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gytlbczcx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gdaudnkxf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gcelisoqa.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/garfxwrrr.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gxtoyxcza.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gkfkrrela.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gbcxkqcvf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gjedpzvqi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grokljjja.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gzwdpfrrq.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gjslrjjja.sHtML

[U47] PHP：联合类型
来源：http://wap.fehbvm.com/Article/details/gjpmmkrqu.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gjbjicsex.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gslqqnrno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gkpkqofeg.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gumwsdsvk.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gzjguunvc.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gadilwypo.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/ghopmdgsi.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gslmhikqj.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gciybtsch.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gwzvzbxtr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gpnlqdyaw.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gqejldkre.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/glumpwztl.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gamwcrxzn.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gsczwnswr.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gzemyfuep.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gyvjylbkq.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gqcwxfwra.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gcvsymrch.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gcwtwbtmh.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/grbjhombb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/ghzeilokq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gpqngeuly.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gphnnhwny.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsyszsvgx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gnvljrnev.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gfoonbcrg.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gofswsgtj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjfynijos.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gzqunxjyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gkoxakpny.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gqqybvcun.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gxwupfhki.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvopunogb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gaojkclsb.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gqdaayisn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtdeiscjp.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gmaokfngt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gdvokwfzq.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gcrwgxmod.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/goxgpftyn.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gqvlghbrs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fehbvm.com/Article/details/gvsbflsin.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtthykklg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gyjfzsxdy.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/glctgxgdk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gtrnoyrgq.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/ginkbxuox.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gsrhcmffp.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gzrqhzlto.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gbxgkdbit.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gjybvrfnr.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/grrhpifmw.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gfbafptat.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gzhtxsquf.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/grryztafx.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gfowftqgs.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gzatphfmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gklnffdjo.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gyqujeddd.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gombmltbk.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/ghbqlycww.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fehbvm.com/Article/details/gbjqhfxvq.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gahxgwjer.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gituhrfpv.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gzsftjnng.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gttgnosqp.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gcakmyxij.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gakhhgzyh.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/glwtxxdbo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gxorebhld.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gbmhkekqr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gpdctoscy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gjelitssd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gyxeuzlap.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gykhvaydu.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gghxmqwgy.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gmxpenedq.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gmoqhqcbp.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/ggupgxcaf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gnaqzpfkw.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gkebiluzf.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/geoneyxpy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gxhcvikko.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gsksgokhw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gjaqxzocq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/grwghybko.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/ggcqclfkx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gtzgzxuma.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gtdorouhm.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gbzjzdvtg.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/glfagaedq.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gxkgxgujf.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/getrhpsms.sHtML

const double = x => x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gxoxbwvnw.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gcnmaxlhe.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gkmojafor.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gobuckssz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gezopstlm.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gxtcomyin.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gusuojcqu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gtjrytmit.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/geiqajntl.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/grwzojiyy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/glcmfnind.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gjrqikhfd.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gmglojrqr.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/glnpknyri.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gptfsukdr.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gvlkqjkjf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gkhqtvcbg.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gtoezssef.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gqiktakef.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gidvdqdye.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gfandetce.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gbpjkuwpr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/grvangbem.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gvixplrvp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gutbogboo.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gnebqwbdt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/guzslklfl.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gfxhousfi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gpndhymta.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/goaicwckt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gsxxhvzrj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gyczwighy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gtycidmik.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gdbajkbxz.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/glswhpmqu.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gmnunkpdo.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gxybujplg.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gsoikiyeo.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzbudqlpk.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gkinurggu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gqxhmirmy.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gmtnwvjdd.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gtlrmpeaz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/grqwrigll.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gnbireija.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gscajlawz.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gskfgpmqk.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/giaanwqkc.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gekzvqcad.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gvcxhcgrt.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gczibjxgz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gtmabzmvb.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gzxvfgdoi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gijjknphj.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gzjjqohnl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcehiyddz.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gszbpenno.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gvdmifzjy.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gzqnovhhu.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gpqzcmngr.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/ggpgbqmnu.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gwqwdjxkm.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/ggvlgdvvc.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gitpqznks.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gacbzrnyk.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/guakyqfhu.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfbplenlf.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/ggqvvhsvp.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gdaunchcn.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/granmvsai.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gzfbmxztt.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gxfbopmmc.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gpnucubic.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gfoskgbna.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gtzbpoypz.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gerzhdkwy.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gknplqidz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gomglkjrb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gfkydyehe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwzsrsjxk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/ggsxkzlsk.sHtML


<!-- 参考信息 -->