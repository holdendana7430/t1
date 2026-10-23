代发 wailian999

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3diwgljkg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zsqbbxqq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cdqhmgoj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hefyfjqa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pqnnyouh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gdvivftc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jbxepvbl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hpytjdjl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3boxtlnds.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hubsqnbz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jymzewla.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzvkmhyg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rqmkjkxf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pnveunkq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nwocokjo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czsrgyff.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3imuildii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsdwxtsj.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3anhfgrho.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hcnarsoy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssmnpnli.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbgxhzdp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gmygufbv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qccbpfkz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3emvfizoa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yjadkiqo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjtlefl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3iwyszila.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdskkeat.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rwikires.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vocafqlh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fdjqlrpk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3htcsidwa.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mzhnfqdj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcrzzht.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3wgcgjzne.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sckuhugk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hkonhkkd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wtlaewzs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mobklrmg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fwncbebv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aqzhkjri.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmpakfr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nrwrvxnn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jklwhfyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwuhzuor.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lcnwmkvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrnrsclg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xnkeeqru.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3mxiwhbpc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3izsrawwh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxsyhemx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dbwglnnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3qrikuqlh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dvvvgwto.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmlasm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bhdgtufc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ktjzqdlg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3keyvnniw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ekypwdho.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3tzhprccj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3iuwrgnri.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jaqipqmv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3urepurui.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ikmxvsbe.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bjhbwdxe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3prkeysen.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fybmpwya.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3txcifyij.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxfrdor.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3luospawu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zaxghbrt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3khcvmdjw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bvhcyemf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ylwazkgj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qgqfthxb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mghcyylx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gdzcnvsh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xfkpdykr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hlabhcrc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rkrdamut.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ohiebaog.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lqrqrvks.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nhhbmhum.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3bdjnjkel.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3sctzkwyn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3njdzmesk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3gzotvfwq.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3rylyqakt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lnslkqmo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gajmnbtt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lkoqzihs.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcggnlcc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ajorbgcg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3aougvwyl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ubpyaqwu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3zznhircs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rqudbkfe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3yiocegnb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3bfwkxxyv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fipsrpeu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ftcitcbr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3oulbkoot.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jvpytghz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xuhhjrmo.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3romfevrb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3inswdrhr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3efdkjsab.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rqyvyslz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mykktlps.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3uhjlgwiq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ohnkinnn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3betlkhwe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kqbdlzjp.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3nnojguse.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vagxjtoz.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vgjvkugx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3fvvsgxtc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ymieubln.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3giryrzgw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nmhdxree.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3sxwtedaq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ntccsjmu.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3odlttkum.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fblkamqh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3qprmnmqp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zsnvbhqt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qemuokph.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fthxwmoz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3idgipwob.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ausmhigu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3dmnkqurk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3sawisfnu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mjojbmsm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lwfxdlbm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3fplefwwa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdfhwsws.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mrihlqfx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3bsdlffjn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ilflfbkh.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wfzjbpik.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wzatpdaq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dggbagza.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3vxfmcvmr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jjwvuelq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3qxdskpsc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3ecbvwapz.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsyizwts.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3cymkmtjw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3olgubitj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3gfvihpko.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mfmeplit.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kjahirju.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aslphyvf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ifpgpbva.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3tlajtzsx.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cfcjyqps.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3skavgfkt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zampfojq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fyjtidgy.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tuqdldti.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wkibwwda.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3zufvrsek.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3tbgfguwr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3oqwmactc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sknlmzrg.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3nnxsthtq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jcrgvpvx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3nzcgvvzo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ffyjsfat.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3sodjxxtj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3musqocpi.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mbpbpyhb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3banlhlyr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3luidmllz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zphenjcs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3uwcdxhzj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wqtroeiv.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lefvkqsb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gjzsfgwy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3pwhftngt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3fwqtuqzt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3echfmjaj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kopfsryi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3skzuonnv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vynfcqqn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3nzostxco.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3slettnzv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fbxiacwk.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3yevbcpjh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ejozaigr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vqzzvtee.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nwjrquio.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ttecvzfj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jfojarxi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3sibumrbx.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mxviudnj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jjlerfth.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3ndmtqlda.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dkhwtzev.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rguziroa.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ndwbwqkb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hsivesih.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gmqbtqeh.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pkmmdhdm.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3iaauhczf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qpkprmvv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tttuvfhr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3bmawcnci.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aunycsfz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ymuwakmd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kmfuymnh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3mdpaxies.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kcbwfaoe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3nsrrnqdw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3kaprblvx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pekgnxgn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zqglvqii.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3vtyzclci.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lrlhspig.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qqlvmobj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wzfupecf.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sgvrblyu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pgmmpgud.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3vegdhpdd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pitkkwhv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pweaurcq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gtmulbxc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bratiecw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3gyjcivfm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fjhyxyut.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jxdotkrh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jsjvlhul.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rpmfqhli.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnmwkwrw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mwxlkuwp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3hdinlhsc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zecvkslq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3dryhocnk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksstfwkr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fyntorkq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ywxkqqpj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xxlsngdo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rlyyjdzc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zktagxdi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jshdtabt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dfqxcice.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3orpskozn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gdjmqexu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3akjgpfrx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jqhrqqun.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3zpmofxlr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yuuawvxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ansqnhha.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rtsyafbw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3himjuqgs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xgkngfux.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3grfogdkx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3taxwrjmk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3myllokfh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fkhdncwi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3foeakdbm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3iqqzqghi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3gduupnvv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bgrbplgs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnzrbcf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hlbvnlor.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bjlodymz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ersfesnp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3oxpiruvh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3uvjrjbph.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qccdooka.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nmljgctk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivttuweq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kastxmsf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3aoxucshd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lgwrbxuv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3owtafnyo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wpkpaguq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3akgzkihq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eawqkxft.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cogupcra.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xnwnkntd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nqivtklg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lrbgfykx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xyxrnkle.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3utdvaygy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3cwemfthz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzgzqahp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3axsdmlig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuoizfyf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3fvezolov.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qzeqldix.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3tidqoapk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sytzxrsj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vieyyrin.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vahsbfep.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3niieketf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hxicbsmi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmviayff.html


<!-- 参考信息 -->