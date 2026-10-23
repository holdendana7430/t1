代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hfqgnqzi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3sgqllfvq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rbuykpta.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3iughqnfj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tydbeyoz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vzvzbmvk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ncgfvgkf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fxufvlkx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bcchivau.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yuajvght.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kndttbfw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vaxugavn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pagfulji.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pcwmlzky.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hrmcucsd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veedihsr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rtyckktt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lzaihgrz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3iypookiw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlnimiw.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ncblvyqh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3apyxttmf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pvjdadkz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3nmsylrey.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkjbyvaq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzkuiufm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oizlkvvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3igawdvvx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaheggas.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3codzjwqd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kkjddlnf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fndtkvps.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jpjsdnbn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mjiwolbb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xvvpndse.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ckjkieif.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3isogtbzu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nwnlujgl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gltwhdal.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kpfvkrox.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rslopsle.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3efzejapm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3atgwvwzk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qlcxxvbc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bunylpwu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmgqmhff.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jyfnseap.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wiuzauqz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kbtgvase.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbfwwrum.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgmytdfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3veujsxyg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3omjaezjw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bbglmtbm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cbcxuxyi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cnfhajit.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3onhmmhjk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jnelwxdj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3nlskhvrj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tqhcngfd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kuvqsruy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qjcjjtla.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3vbutewct.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3alrinxdk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3klaoefdp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3vhylxjbk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fznibgvk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nwctytgd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rfgtzwud.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xsmxherz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tkvwohcz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3axdlydxz.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vtargenw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3rwpznotb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mryrfljm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ymhuhmhk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3rfptxsfb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fxthuqgb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tksexjem.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdgqudk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3dtfqhrwc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3boiewixd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rjvpxmnk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3csenrzit.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wmxszthy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zeunmrxx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3umggtntb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qnuxprmy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rxaaokmq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbtzvbtz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3twdwoqlv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fpsygvaa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ykumqnna.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ikkwkguz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3zslgttnt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bioqirlm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3hihyhewn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3teyluzmy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vombpjor.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aplkszko.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3puxgoimk.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvhjxzs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zhugchli.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ahiwoxku.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kvpdhfyd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3onadxlmm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3isppqgji.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hjehbklp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ibhaojxj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mdlfpwhn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lizhqceu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3suiqxjqs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3xhfxadgg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3fvwusvbz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mohqthht.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zifrrhxq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3jgvxlahy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3uifwnbju.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pbtwdxhb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bhyenmgw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3zztjyyqn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gmhutmtv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ecoxbdgg.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nlpzqvlf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3sjvkytvz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3datqcgsj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3aqygvwdn.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sozwffjj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3iqcnimif.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dsnikuxn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wxztwxis.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjozoduk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ntcvhxqy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3rqcscdqy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3cagdthlc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3zwlteyml.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aqhhvzya.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yvdbmgvy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mugjektz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qgnzcdpk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vodkvyde.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpvrlqtu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ynlsjyfx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3fgscfusl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvnicdxz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nuttivvq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3podhhvms.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3pljtgcuc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3wmcgfvyu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ikxwbjeh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fdivgxop.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmsqrfuq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3tziqrfmo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xslxqclh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxtbowsd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ibqfajdi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3fuzlkzyq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3epjljoit.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qygxzlbu.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pnesorsm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3iippzdjj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mvyrceyi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jetdtkdv.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3loimceiu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ubzydnqs.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfiubqsm.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kwvmxeig.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zkiuewis.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gfcpukpd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mrtwzvkl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ljeemjgq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cwimsdta.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ffvlxzzd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ejanxfcl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3bnarqjxb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3kxutkiix.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hbwlpsoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ykxcpdci.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fydodklp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3acqvzgee.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3ydklbztq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdkxgo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qexsksfl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bawaskmq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3yvphpxdr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3njgznvgi.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qbqedtge.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ofcqxxxd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3oouhnqtb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3bxdsnofu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3uvpftrvs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cbrozzim.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gzexsixl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ephqcifr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3gzlpzfxc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3rmsotyoz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ojjhgjzb.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iqxvxpht.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eukbliai.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iurzwbjj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjagfm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3clhdujyj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ixuavxel.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ixtdszjr.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3thjsjotf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3drwydmwg.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zwdopzsk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3dgodlovv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3udwglypf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mfdyblye.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3nlfxyzim.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3edjrutra.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hvgvifzc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3shsstxlc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3azvgboev.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3mmcpaqtj.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nqhmdakf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eekjoobw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3xvlngdsn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hcjxkclx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3xqsqedzo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tjjnngct.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3inwbhtse.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kwfhupnu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3yabwqosj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3oydwwdkx.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bqgmutiw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3cuqurtfl.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3ltqgpvrv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3refpqhep.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vdjahuix.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mtaonyou.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3zripdwdf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3jwxiqmos.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qpgmvzmv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zprgcwui.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yxjmjhmj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vwsmezpc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3epadwsfy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bgpgtraf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nidwowfe.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3blvevgju.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xrhevdnk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vcqtuyso.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ebgxjrve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pdekfgjm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jkughsrr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3isenhhnf.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tbvrntzi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3hbjhmdtd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qsbncugc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fkworilo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mexuezad.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3cofqwcrj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zgizorno.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3yvtqergn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3fhydmrcj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3byobehwm.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vugbhxcq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hpgoqmbv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wytljmbw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3blefketu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lahjlodb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kxwqjopm.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vlyckybd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fsojyzrd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3erqvtnji.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rmohhymd.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tyslwinh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3utjrswlz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kgaeulva.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3nyberikf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3pflflukv.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gkufjbpg.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3smwlhorl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nbibkssm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3jkezvrfy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cskporpc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bxslbwmk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3twfegclr.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kcvcbuca.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nppxwlnk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ohpaefat.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3meqnitam.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3deifngbv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ihjobuzy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3frgaijen.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ceidjvhq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fwjlppdw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3irlfzaec.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ncfuzsed.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3edwwduif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swmpxvsk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3conivccw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lagteqqe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zrmaviyx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wrakfszi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gbatkqdx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yzcpjptl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pqwmkrum.html


<!-- 参考信息 -->