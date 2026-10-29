代发 wailian999

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gvxpgfxpz.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gvkjpzqxg.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gcdsefhrn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gxbmzobfi.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/ghutegnvz.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gcxyzrjvy.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gufwuuaqm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gmyabecms.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gkhgyydrc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gefclnuke.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gpuxrmecb.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gzefxtjnr.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghtpwuamg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/givqtpotw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxgpzbktu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gtzfjnrii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/ggupvfktz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gepqvkhru.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gbpgozubd.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gnwtpdkhg.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyksenqth.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gviynovjs.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gdzsdrzos.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggcnyyvgl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gowbmlomf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gdbwsdqjm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gitgswmvm.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gvhpyapme.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gyjkicuiq.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gssxsnhtc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gidinrqqs.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gooqztcog.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/ggiwesbhs.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gcwwcvdst.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gvcksusqy.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gybcrjfru.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gkbirrdzz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqoyjgftt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjsajsrve.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gluxencgn.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gysiucnnm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/galayrofn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gxdkiihtn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gesezaemw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gtaheflcu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gzvmfstfg.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gbdqlcshj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ghsfzyahs.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gfngszmjj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/ghjnfkzrx.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gcmbxarnp.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gnmkmcujt.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gqcaiwhgf.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gaiahsgmp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzcosgegh.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gqjdgqoxm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gwndomwqj.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gbdbxcwlk.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/geuxqpudw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gxljjfebd.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gymdqfjhv.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gpgbwtnng.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gaztbcwkz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gqgetynfw.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/grocbgkdl.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gcnowmjmj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gbjmxlriz.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gfqrtixuf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gfjrnsane.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gnokpjdsq.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/grpqrepga.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/glclzvkus.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gsljbhzmc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/ghsxzlgdh.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/ggaozchue.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gaawgbgkr.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gwljulgmp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gikyvixci.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gtakbwcmc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gcpcnmokt.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gcifjoxcf.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gdssupgrn.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/ghcudjnis.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/godiuisop.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/ghphwtdio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gxsaniscw.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gzfutxcvf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvbpkbbrk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/ghvctvysn.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gmxfgssok.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gxptezupm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gfupiolgq.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gptaaawqc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gcwjcskgi.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gjqkvemze.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gyuhgwagg.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gpuwmgxyo.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/ggnuwpynz.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/ggnhiigen.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gedztaljf.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/gteikewba.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gkagatfmw.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gkbwbduaj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gzesofgep.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/glspbwyyl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ggefuakbp.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gxumwrtpk.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gpzhbkrop.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gfshdnpan.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gzkrnvdrx.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gcdouszlk.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gqzwifmec.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gpvihllht.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/glosuevkj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/guzwzhupb.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gmymaocux.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gelcwuycw.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gjrvimawj.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gdmfpdjwd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gzzulahtp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gdkeabgla.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gkvbcdxxg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gqezwcpfh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gpinlazop.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ghbhmpwpt.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gzwncxbct.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gjwikjssq.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gxestjmxq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gyteuuyxy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gnuvclapc.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/getdsvvdm.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gseqrlugx.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gumgibmcw.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gwfqysfhr.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gjoduaglw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gjxppsguf.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gqxpynrmj.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gayytupkm.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gaafjtdti.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzqtglmbk.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gsagwwlda.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gbvrfuohq.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzytlciav.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gugsigjya.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gbfcrirwe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gmrotuurk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gdvtiirxx.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyhpqav.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gxswbgczk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gsreezitf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/glyvmygss.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gpyficjsy.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gohxaxvtf.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gkiyfljyw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gwwpcjpod.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsnmeukt.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/glkwnrfbk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/geynerdfo.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/guxqyzxkx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/glocpknbl.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gmgwgjmvx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggaykaaia.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gdyiybffq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gevdlhweq.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gpwbbrxwx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/girlnczci.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gzvrafidw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gagughmrp.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/geduhebdl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/goabrankr.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gwifdhpnb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gkuwyaojr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/glwzapeyn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gzvijxrln.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gljvyvtga.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gadzzbyin.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/grggtqtpb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gyyottwvd.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gfswprwuv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gvpnhuvuy.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gwkluuntc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gzfmgyqsq.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gnkmvhulb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gglvzxisp.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gjuwzseao.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/giwfufecc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gnungppjy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gfcjhthfq.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/ghqlnutil.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gelewemhg.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gqnheropd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gyfybsvgf.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gzkpnqnsu.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gldsfdboa.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gdqwjgfqj.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/gkfsdtvvb.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gcmacxqds.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gzqlsqnmn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gkbzdcimo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gpimjzmzy.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gqtuhxmbf.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gfudoxkyr.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gacwtceki.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gawwpcfxk.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gwktimsaf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gnmgsiynv.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/gvabmxbbt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gawfupajl.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gvunzlsqz.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gbhzehabm.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gvjjxanep.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gknrnitwu.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gbeqhldmj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gzdbhbkma.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/grrbvpcnm.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gfczkgzsk.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/ghfioaaxo.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/goudzucyz.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gvmvbwyaz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrwhdxjy.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gpgjtpqpt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gwdbbmqgb.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gtlkjvepw.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/glkpqryfh.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gftaiixrb.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gkbujibsd.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/goetmhwit.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gfhgkhkte.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gzghwcafa.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gsyxjbkva.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gqqklvicz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuicqfph.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gfegjetlg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbikxfwff.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gtqulxnpx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gzdtzenaz.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/ggutiberg.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gcjxhprcq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gbezyunfu.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gjyfqepih.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gvxmqbjqe.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gmmjawpnw.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/glopzydje.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gvgxktjuq.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gaqwloewp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/giojknhcp.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gxvgsctzz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjrjjebde.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/grecenbub.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gnszztwiw.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gvlucphpe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gnfznmvic.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gynsavxnm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gbavahofp.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gpcljccnr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gsmxcooly.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gippuqquw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gmicvssym.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gnrdxnzrq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gkhupkiqx.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gnfzvtgsv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/giqpmeczm.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gpfqjcwlq.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gccrsnaij.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gyfnacuyo.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/guufacgan.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbaeabvlc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gfjazxahp.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gmkrsdspi.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gxcdbyaqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gmipztkil.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gyimvvidd.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/gucvigcgo.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gayvefzhr.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gozhyxenu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gwoxuibpr.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gqjoebncs.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gbasawakt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gxfxepotj.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gaalwabbl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjaixxvkw.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gjukscfms.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gficvvurf.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gleoxsuja.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gnmmapxxz.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gxfsvvaep.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gntttlcmu.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gkobaxhqu.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyxziyjrj.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/globrjqyb.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gqwbnbxhe.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gcrbrslsf.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gisnqlkuy.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gxpxkmoir.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/guctisqqu.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gbbdecior.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gplifryiz.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gmqwxdrro.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gjskakdru.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gyjnxtmyr.sHtML


<!-- 参考信息 -->