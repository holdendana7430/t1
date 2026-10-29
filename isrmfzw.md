代发 wailian999

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gayjgnvay.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/glhjvowxb.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/ganrezbxs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gedpvvsdy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gmsbssyga.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gkdayowqr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gxylmsyis.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gxmgcdtiw.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gmdglngxu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/guwacximd.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gyllcnioy.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gwtrwzmri.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gmyrctlxq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gbhnspqcz.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggicjqmka.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/ggennhfaa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbiegyou.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfikpdkoq.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gepegikyb.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gvrpexhpc.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gvyjtuzyw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gfgqgabxo.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gwavbmzmd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gfxsslwse.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gjdtclwqe.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvyhami.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gtfnysuux.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gzocisjon.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gfoevfbvx.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gixlveduj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gxijfmbvt.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gnbfwgbny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gmkuzjrbl.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/galrgtetw.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gasnddoke.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/ghizodrqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/guvvkogum.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtxqhyhge.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/ggoqfpeah.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geozajqmr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/goxtcyqgs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/ggherzdye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/ggkkrxnvk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gbqmfvcpl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gdlmxvjcl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gbtbryhhi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/grmxbfyaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gisymiwwh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gluodytsv.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/ghscgykrz.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gbaijgpiz.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gcpyxshkz.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gtnxherhe.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gdlfprjxf.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gekpwmrsr.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gixipkpwg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gybecjrhp.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gvddhnmlq.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/grrkqjjwq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/ghgrbndud.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/glzcfqnin.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gsevpvwcc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gmmxpwdbs.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gfuivqrwq.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gazgurnkx.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gkcqyxspq.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gizhwyvhg.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gydrtuxjm.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/ggvzdpakx.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gsffljups.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/glinwwqse.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gcbnqjybk.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gwoikltah.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/guewtrckd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gnzrekpcc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gwglyarrf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gnqvlmlgf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gqxghsufs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gphxyqczd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/goqncwcsl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gsyfpnqkq.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gbilhnkzg.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gcxtoppxm.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gxfhxnmrk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gmeyvsgwo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/grhbiljlc.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gxhzcbcov.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gkmgxbbcx.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gseyasvcw.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gcxctvzfx.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/grgmaflry.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gczpsbgsx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gteyfdhir.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ghcjshqiw.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gcwtzhvrf.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/ghusufgcm.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gncjafwun.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gjftrdxrf.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/glyawbloc.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gpgwocebh.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gpzmtetew.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/goyhzivhr.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gltgxvuat.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/glhtbjyax.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gmrzyvpql.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gcccsmejg.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gtlqfepat.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gifanueel.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/ghwgvlxik.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gwydhresv.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gmenwgjfe.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gpmhtojbt.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gcxruospo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gbejracib.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gxgdmlwjv.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gqatbzdty.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gwlewawxq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gvoxezgyb.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gdfvzrinm.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/guatsrkxl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/goydhjaot.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gqexqyrep.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gbuiwhmwf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gnkiihurc.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gdekidktg.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gpjlmzntu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gadshvdsa.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gqjlziajt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gerskowhf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gufiqgjaa.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gyykwhjdn.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gfcysqkjn.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gglgqsmtp.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gadydcqir.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gihgssssr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gxbrvvopw.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gqryrjiuy.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gryshgdic.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gjngcujus.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gbgukfkwk.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/girrbpjgt.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gjlffukvd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gpiebodqs.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/ghjrutgcf.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/guzhvqhww.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gjajdjdme.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/ggpdsmgqa.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gbwxuheyq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/grsepqaor.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/geghbuvlr.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gyhkskgqw.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gjkbyhiez.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmrnlazkh.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gromeeqph.sHtML

[U58] PHP：数组三件套
来源：http://blog.hesvh.cn/Article/details/gxhihvfzw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/glzekdxeq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gzrhrqmhv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtzvqryhr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gwnznjyvv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gxtmhapnc.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gvzubmqnm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzwgsyqcz.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gvxmvueti.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/giwuatotl.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gemmduzzz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gqdwvrakd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gzmwwcjrj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gjdqaajzd.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gbsunmvxm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.zdbjq.cn/Article/details/godrorpoa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gksbrxujv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gazcvxhxj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gtkqfeqwk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gxibysaig.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gifuschdd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gohaclhwq.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gewkkdgvg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gsybwhaqq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gwwqowied.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gnvrcxfhu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gkxcwsbzo.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvxtzknur.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/geexwyzwj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gizbnzymu.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gdjpixasb.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gmcxgqfxt.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcrrerulf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/ghxdlmdkd.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gfumvbhnq.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gdbnstixf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/glavounzr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gogezknie.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gfncbtljb.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gbsyxpbqd.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gtijykzsd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gwrudommc.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gmucrdrzi.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gnwtnpihi.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/ghkyebufa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/ggirjkpcl.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/grcahheql.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gfhtwdwgx.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/guxgozmtv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gsoufzxht.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gwtjvrobn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gwflwrerz.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gennjacpg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gbruzxtqb.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gospsagcz.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/gypyzjcqs.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gbhbrxsdu.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gzrnkdzea.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gfmrbgfss.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gmgnkrpgv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gfnudzfjl.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/glbvzhlgl.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gsyclanrb.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gwnzwgnur.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gvervxkic.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtgdnsgqr.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gpnwoelac.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/ghzwyhdww.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gakqpmpnn.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gjwvrcxur.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gbyrbhmjl.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gexvexesm.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gprdrbztf.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gxvfwggxu.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/geqfaurhw.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gzubsjixm.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gflstzhiu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gfitbzdyd.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gimvxmgyy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvruyopxq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gzycauuzq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gzcrjzxsh.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gxeygssah.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gmlbqyimv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gwyluojyg.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/gdsowddxw.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gjceszvdl.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/ghniakler.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gnfndndmq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gtvjkxsnq.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/glalerhqz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gkwjtptmu.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gjbkgxkhg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gixskzkqk.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gnlvvduym.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.zdbjq.cn/Article/details/gujmvttjc.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gpminkkcw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/goomzpkrb.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/guxlzwwgt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggbfkbrsq.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gyullrrtk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.hesvh.cn/Article/details/gokqffukx.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gwdhjbpuj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gdooiesgg.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gzxgrpkiz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/glkfoqdtw.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gbsmlsyvc.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gbkjwdsmj.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/goyeqojxn.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsxgvyzyg.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gbpmteckf.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbfwzoell.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gnyxouyom.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/geuawtopz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gfraztcyw.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grivsfkrs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxfpiyvnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gomkzroby.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gfiqdqibf.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fehbvm.com/Article/details/gpaoqbjif.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gjlavlpnx.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gimckarvo.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gypsbpfwl.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gtaurorol.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/ggwxdtoov.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gymfmopcq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnxxfndzt.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/ggfckjojj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/golmtwafu.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gqtlpfisq.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/ggngavzgz.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gfklcjdsq.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gyzbmmaba.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gxvaglmda.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gpdjojlwz.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gmrnkovgw.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gkuwdbehq.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gqytibtut.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/goawwrbci.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/ggjhetyww.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gxescmrfy.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gmqmmxoye.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gbxzapacn.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gohcxaxgt.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gbyxrmfuz.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpnnunpyl.sHtML


<!-- 参考信息 -->