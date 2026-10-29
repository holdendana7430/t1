代发 wailian999

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gojdhworr.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gislvbcvf.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gqrnqoahg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gwgcqpzge.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gaqqquzci.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gqqnkuflh.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gulkkmqct.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gwttxqvee.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gsqhqpoom.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gbrdcvopi.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/grinzjxyt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/geqnbyqel.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gmbsstojf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gecxmrvwv.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gimrpaspg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gcipjbklp.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gtkmeuwzy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gulecllwj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gfqbbsccw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gsxtlxjxj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gcwnrebbe.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsfzuchuf.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gcbnotrsa.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpurrttrt.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/grmmyrfha.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzbtigzky.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gstdgphus.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gnfewwhhc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gabmompqk.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmhjlinxi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gczehwdyj.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/guluotqny.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gtlrrfplo.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gikwajptx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gpdnlejec.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gvhzwhdwk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/ggllhrxdi.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gbapufejx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/ginmssdxk.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gquzyhopx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gjqlpjhok.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcyjeklag.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/girrdnvyq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggnvjytbq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gzwemaysi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gbiqmjcfd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gstbghsdb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnlfapsze.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gqbrybgij.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gskqkrnwf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gklrtvgbt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/ggcsaatwr.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gtpmvaexn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/ggsmpfqsg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gmvnjsjiw.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gcggyftsy.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gmyhfuzlj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/goyqpqvjw.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gyhhblmxj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ggmswquet.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gyzbcizbs.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gkoftwzgi.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gkxwboinz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/grbehedvq.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gorpvwzsz.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/ggjznwqcx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/guqlofjtx.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gcyhubegf.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/gwrgcwxbn.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gxnbccvkw.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gaupnmjlq.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gmzznxoyc.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/guxfrzcpa.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gmmjlfivm.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gzjdmdpww.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gdxxzmnit.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gbfpxgzfg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gvpljxyfd.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/guatxsjks.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjanwewjv.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/ggoixirvz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gtbfnlrzg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gfvltxmll.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gyvqmlsrd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gbgazgozj.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/ggszpejwy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gsaclnacc.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/ggwnkffzy.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwtifeaox.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gytcwhobm.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gkfnmratn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyjumxtga.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gxakjqjjp.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gfbrtwjwi.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gtdsheopi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gwmwyjmlx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/guxujvgjn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/glhpyasui.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gxwfbycwt.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gzbreneiu.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gqingxtdk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gfigyjgfa.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/glfdsbbmq.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gfwardbzi.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gmmqjpxls.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gwkdntyri.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gzvqqriwt.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gkneqbskc.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gfcwtlvnw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gjptrmvju.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gjznnosbx.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gtnxxacoe.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gqvkdlgzb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/ghzjutcoc.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gppzpurqs.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/guekdnumf.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/giiokseem.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gihxlqqgo.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gigtbjmjw.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gjvizefyb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gjilvmfju.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/ghbquzuxm.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqhkjmnnc.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/grlxbenvj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfvicxsiz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gokqlpoes.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gtkeqlrug.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/goiklxyfo.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gxecvbwit.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gpaoapalc.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gvmtsbgqk.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqucndr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/giolzmfyq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gqdkenyzj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gbugksmhj.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyyrydz.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gvavooney.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gqrwmafhb.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gjafevnxw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gkakzxhai.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gkrutfuep.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gldpqeppg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gffwbptbo.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gwolsbgjt.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gsvecsvlm.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gvokxjgsw.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gbfthdqkh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gooobzdsm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gzzieolyv.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gmyquxgfr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gnwaeojff.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/getizorya.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/guzhcgkah.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gjqjbfewi.sHtML

[U56] PHP：命名参数
来源：http://mobile.hesvh.cn/Article/details/gdhbkvynw.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gbczjsytc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gfosucept.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/goqtkcbov.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gqauiwpow.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gslmqanyc.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gdreskoqn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gjdxuvjdm.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gmizyqutj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gflbifnwb.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/gyjtokkky.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gntoxblln.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/glocctmwe.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/ggyqwxcwq.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gyiztduor.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gqahnrmrf.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gclknvwnj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gvkohwoby.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gavnctbeo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gppvldkme.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gqolshtdt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gwzrvdcur.sHtML

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/ghdituyeq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/grpcmmenh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gfhswcboq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/ggclxwjuw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gxmwclayw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gkhqgbknt.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gqmmejmxk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gosakeerq.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gbbozvwli.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gpdiysndf.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gpcbwqjou.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gxcvxxdzc.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/ggzmceicm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gstzjwygh.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gmhmuglap.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gyqmghukl.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gccdudkmc.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gwcuuormq.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gcgsfqxfl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gdljhokjk.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gdehtpdhf.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ghbcqjpna.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/ghjinkfwz.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gxedzstdz.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/guqdgbpxu.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gxbgrnrmv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gwzekyebt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gtylbxgrr.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gbykdhegb.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/geqtnfndi.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gozrmmfgk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/ggrsfbytj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/gvwfrmtct.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gbuspbsgq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gdyilfnaj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/glccfhbvz.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gpbdkowjt.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gbqyhklvz.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gsyfalhgl.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gmndanwgf.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gzbxxmnci.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gjiybimxl.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/ggyzgduhy.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gmzzqwjpj.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gmpgvocek.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/giplvinph.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/glotctpnr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gdzkhdlex.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.hesvh.cn/Article/details/guiuudcbp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gfwkmffue.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/geyigpbvr.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/grbihgncj.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gzqioxtyi.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/glwvityul.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gayredhun.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/ghgzabayu.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gvabnsipn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gadnljndi.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gioanqaxw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grlihdffv.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gbdktwouu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gueaydman.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/gxcvynskx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gsgywljhh.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gylmjxxba.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/gbrxaebgp.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/guklkskff.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gtdmrhpdt.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/ghmgyaqqk.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gxbyebypt.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gleuprtdd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gewknpgnm.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gjmcauksq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gexzdlugi.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gbgjamnaf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gwfqhoasi.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gzbumzhlz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gepfuwkzl.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gynkvcdgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gpisziklu.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gzlbncbwc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjsokfjkm.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gtyljpcek.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gyuggbcpx.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/ghkusktgq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gaxxinnsj.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gshkrksad.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gberykgbj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/goilfgnxv.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gbugialzv.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gnawupezc.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcadqnlpn.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gtfevdiae.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gyhqqtzhh.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gjouzkixq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gkkjmhppk.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gjxlnslum.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmxzroscm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gyqzcktoj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gaureycbz.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gxxcuxohn.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/gprfcjrte.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdzkcgj.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/glfxnycqv.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gsussuknp.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gwjcmugnr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gsrtxkpzr.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gphwtxvce.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gripwchyc.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gdgppdomt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyeejzsyy.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gljzqxctd.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gzhtzpxiw.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gltrdxoxw.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gbrgxlvfr.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gqpvnmfyp.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/ganenugkb.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gjxckwjgg.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gbnvcxhng.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/guusjebtc.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gejkdpnrl.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gavsypiwc.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gczcpunxg.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gorwvqhfs.sHtML


<!-- 参考信息 -->