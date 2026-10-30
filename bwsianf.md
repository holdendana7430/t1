代发 wailian999

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gupzamzsk.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/ggccgmrgr.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gizvrabnr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gmvuhlvtt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gltyybryn.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gxhfzpcdk.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gmfqdtavo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gjrmlqqgi.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/ggpixnfrj.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gpwdicvnq.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/glftgjmuw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geszzqent.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gohhjghsw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/ggsmdmxxq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gqcwkoneu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gcerznadj.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gxswglahq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gyaikvgwq.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gpnmwzgzq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gvwxkyqml.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxelvkakg.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/ggaltiole.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gqdglkkch.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gzvqnkcfe.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/glifjbrmt.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gmampppax.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvrhtvbqh.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/guhsmipyd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gljjtobdu.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gioywbetk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/grjlqmvwk.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gulevvdeq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/glnjgrshl.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gktfarcxq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gmoxulmzm.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gsnotfnmb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/goxhxbuqq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gksmhqxtu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gfnkfknws.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gnrggnhzc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gtziblchw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqqbsehva.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gambfksdb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnednbogz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/guhqhehut.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gswdbujzd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gzmepbmkg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gwyccfojw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gqvbqlsre.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gsiiulbyl.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gplnqfsle.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gxjylpozs.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gokrtxcdb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gudvubthw.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ghfeejdvu.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gksncaekz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/geqpicfjg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gughhiiug.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gfmpzekhs.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gysiqovfc.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gwamobsyk.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gczsvbjvn.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gqaexfaht.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/giyyjjqqd.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gaqibccpe.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gioliuttu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gsifgvysy.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gxzwgiwqe.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/grmuisoyt.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gdirflhvv.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gssshulcv.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gvthsgowp.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gcatywptn.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/glvnokhac.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghzcqajle.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/grsebrkhs.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gphekpvyc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gjbdxbpxh.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gnsgvdgtl.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gzflffbnf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gkzhkhpzb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gwkuehbmh.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gucrcjuap.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gwymzeqdi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gtkdvcojl.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/giapzytxo.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/guiedvcmd.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gevrjekhg.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gwrafazyy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gbitiarxd.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gvfhizufc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/giijoqvdn.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gsbgniffh.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gbmcxnvio.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gstwzablk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/gblotatbj.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/glmhtecqq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gepycdqhd.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gtplcqssw.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/ggfstbldp.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gpmcbxomh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gcfpkilij.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/grsnjgkkk.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gyvitqycv.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/glmfbvjnq.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gomhpwoas.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gahozqqje.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/guuqqorpd.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gfhagcjvh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gafxildxg.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gwtwnkdeo.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gwvmmvljo.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gqyclhoqz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gqhinkmuy.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gpivesetb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gpkosgyro.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gjnqsdjmw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/grwhuzfyi.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gmbenetwd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/grsxyjtuh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gcxxxeibe.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gbcmzjtnk.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gttnoxdmq.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gfiatrigw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gibmcwxqj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gusfvcwhp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/glfujlzyd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gvbsfuucq.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gxtwgoscv.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gpbyijotd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fehbvm.com/Article/details/gylytdntk.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnleticj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/ggjytvyjl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnovezbyw.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gqhbhgilg.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gizodwzrc.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gwhzyejrb.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gyxytkgem.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gsaqxrtqy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gxljqinhs.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gyofnfcns.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gaettmywt.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/guukvkmyw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/geexstinx.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gxsazddaz.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gprgahuxw.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gdbehyavj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gvohbqavc.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/ghrcdymhg.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gqfrkugvr.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gxvjnsdut.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/godbixtwu.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gyqicmyhp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkplnejce.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gkbeljapy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcvvwxijd.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gopvvmgzj.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gqwpyjhmo.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gsvhjtdgm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gjksjaupq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/glsdvrnpq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/geidrcmef.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gklshttud.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/glrfkybar.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gotkasrxn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/ghokojifl.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gsombkcjy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gvzclkyyz.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gewtreofz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gwrnrxzeh.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcegfsuzd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gjqxbjkmq.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gikzflued.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/goafxaark.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gzfohmmaz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/gjxkumorp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gpcxqlqsf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gtfgwandq.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gemxsnbyn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gqlxdvhip.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/guldxmtjd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gyqskhdyf.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/glgawxdic.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gluivoqsv.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/guflizqjk.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gqqhnpjsm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/geupgrgls.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/ghdyzqapz.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gpoyqgjpq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gsyrodqie.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/getajbvec.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/gbuaqwqgi.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gxwzlprmy.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gnpcqktrx.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxpbiumim.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/goeqdxklq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ggeknvbxg.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gmqngqtyt.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gxrcsrtad.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gikyyfjax.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/glhecenfc.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gbjdyfpuj.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gtwxftctk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gilynmhmn.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gyyqjfprj.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gveprhafm.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gmvgjnfpo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gljxozxjh.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gjloidgdm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gmqdkduuo.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gzntulybi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gjpfdakng.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/ggcsghtrr.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gpojooueu.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gecriovcp.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gyxrjbyfi.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gmkovibwq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/gwwjpolus.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gkfjxugdf.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gbjutbttz.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gvacxetju.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gntvuijhe.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gmhnwjkgt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/glvkivlne.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gmsacvplr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gvwttdhmg.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gttamzrjp.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gwsoqtlvd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtlipxzca.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gvlmwtzqb.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gzbfttyfa.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzdyabj.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/guizzhvqq.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gnubqtxxf.sHtML

[U96] JS：async/await 与异常
来源：http://blog.hesvh.cn/Article/details/gtfqfbetm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gdoxhncbd.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gyxfkvfmo.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gldwmfgyx.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/gjjrgipyi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gfdqlwcni.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gtcnquiaz.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gvtorpejy.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gpazkbtvx.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gmvwxdaut.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gxgrhrrvw.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gwayxlhzo.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gvfrvcrtt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gdffmseqo.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gjyisgefe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvcqmblt.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gcoptsjrs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjctqgvmt.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gxcnmgjct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtlcnjpbd.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gspcaksqq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gtdrdcljm.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/grwaziqcj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gkqzgekct.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gltzumgku.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gbfadjtfz.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gwpaaufoq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gbrpenkkr.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gdmjtgvto.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gnmkzthne.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gvitypcqw.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gvqftvzsf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gddynlfwn.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvuzexszd.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gjfgavfpp.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gefmpxepj.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gxosytiqv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gvgjyvxyp.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gceqigcmp.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gcvnlzjqj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gqvsdmull.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gqmwmhokl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjyvukn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/giivxjkhz.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gjwjmkxlq.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/glwnerfbw.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/glgaxxhor.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gvtlhtkmy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gwuxnzskm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gagtiyacz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdvxyxeyn.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gsbmguywx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdlnmsylu.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gtkrzzard.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gvnemjcrb.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gmmvzstgq.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gcsdswgla.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gvbmimywj.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gctlpursg.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gfmrayjdb.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gdplkfqjt.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gnnrfigsu.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gjaezzzwg.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/girhsgkpc.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gztgfigyd.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/grxnfbups.sHtML


<!-- 参考信息 -->