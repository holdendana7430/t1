代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ojwmqygq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nmepcelz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mxcwecbj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ueixxepa.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pakfxdyi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3whycqzpb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xwqkqbjv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3unpwezzl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kqlabixr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dlfsbisu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cammctcb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oyehxgsu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3trmctfoq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3peyvjmiq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3utpdsxuu.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssegwklf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kfagpsme.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrrpyuz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vkqjnylv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbsllch.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qdzwxvmv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dajqhnip.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vayorjml.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zhvkgojc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jjvjlmpg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbodyhn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3azpcjzew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hkavtvdo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrmzpcyc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wcozmzuy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vudxamuv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3piwagtav.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dfczqjev.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wtncqknr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kupbfwlu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3euoyllyc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3cwpxpprf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wkdskumn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ygfezttq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tfliefzc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ntpaiqoo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lfhwntkg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ujgrfplt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3inqpitnx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3szyncsmj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3weqxhbiq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jvzlijvo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hhmzrffg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xbdximtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgnbpbvt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjsbmtzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqzjcrfn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3msivraln.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jaseshkl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dcpzeira.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymqozrvn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3sfjgoinb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zmtwvdsz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rzbdjvkk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3przeruac.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3wpwlwfqv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tdzkgnkw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3whrnkrbg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jnqgbbyp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qmzhqkyj.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zutrlmdg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mgcuuhdf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3guftpzla.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ruiqvadi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3biqltrxz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wvnninat.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ccuuhqed.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ipbqmqwt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqrtfjrb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ywipzxhk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xehogmbt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3yfilaula.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gpltoonb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jhbtbrko.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3srfojzuh.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3weiikrfg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3rampjegn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3conblvfj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jztaswow.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ibwxnoex.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3atezmdbn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nxwtnemg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gcsgspkh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rtyiveix.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3jhaagufl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3ztcienrg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3oghychet.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3jjorcuko.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3umtvygyl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3svepiskd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vqzaondt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3fboyfkdq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ujtzhfrd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3hgmquade.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3reflfqxr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rwjfnanh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkdwzyb.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3eylfcccb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qrkraytx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xdeqkiuy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3irbzpccl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vjfizjzd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qexysvjo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3afntiwux.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ntsywmjx.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3rbsqbfge.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3chmsdqde.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ypufzxwz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3gfcxwfeb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3oypcdwuf.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vapsxsug.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3irhkcalc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3htjoajea.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3bluqgdjt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3euaecxrr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3jzksyqrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jujgrznf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bcmejyxs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdfuwza.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3svazmihv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3krmcigmo.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gklqvrba.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3xlofzbzn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hkwzeyvy.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3bzpolqkg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3smuhqood.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kyywyaei.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ggvnfsym.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jfxgkfcw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3kvxewrrj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3scuwwcja.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rbxkjxnl.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wibnhmmk.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3foowrlcy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpkkgeyx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctsqhwgh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dhtcufjk.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xtrtibyz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ycxdpogi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3cddsxtjp.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3utfznafq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3woanacpn.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ivajerjl.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jubfdacf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3rahnborc.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3cfingzfm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gyuaetgk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qbzpwulx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3gucqelts.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3suysynrn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mgzjxpsm.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gbzwmsqj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3kntaucqh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3knfreceu.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3rwipdnuo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3cglhwtvq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3drqgkltq.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3iikpovvt.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oipneqqb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ljggeewn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3eteuuwuh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zpxogkfp.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3noxspxig.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3aaayntdi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iyivnxhw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jdupcwps.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3mzdtvelf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3oywgylgn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kaqyidqz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3zpmknlly.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3iaoprfmk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3obpvycis.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pktojijs.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hruvwhfv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3dkuwqwvy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3jleabagl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gsqzqgqb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3mloevkmk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3finmztmn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3hyqytmbg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3ippztuxj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pursbkrk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kcdnljrb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3iwpojywq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fttzgzzw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gdidmylm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ifefvkzi.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xzenyype.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tamriglp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mxvpumfx.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3midagoes.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zbpvqfsz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxijfj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3fjhxmrir.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3zuaypovw.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ihjobciu.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3jryqpshw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3qysyoiql.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jqzsqmid.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3isobnzge.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3usddggfg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3obadmlor.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3drgatrna.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3pzpjilvh.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3szedrobh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3lxbqslmg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vzxuvbby.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3xwykwrnq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3zjilavwg.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ejtbmdto.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsmnezin.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fxproglx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wemciujr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3pkyuwkhd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3epmxddhu.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3uoxymkkh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qkhsepor.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3uewazyuh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xljfnxsi.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kwmviixy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3ibicshle.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3alyukbem.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3azkqqnaw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3dhbjizph.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xwopsclq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3brhcgdtt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3htjzonhw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3knxmbpuw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fcowvism.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jfzxtqzx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3weitlezz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3vyjhnmhb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3mrhqwwkl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3twnrwjep.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nqtixfhg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3kmjiwrif.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3cvskbpon.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3isklfiwr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uusdedqi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3urxqgolf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qeyccoju.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3yucbxjnc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3xukropke.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pnnkflij.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bicswcfr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lmdnzpmo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xtvndtzp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3arochbzd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hegnpdng.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zpczrkhq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xpgjzclg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bndvfwhs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3nxectrtu.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3daufnrqm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bkzkhfod.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lsowslkp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ehbuztho.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kbhfwzub.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yxxayzva.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ksoecsvf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qdxfxahl.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ewkbbygk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xzamidvw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qyttvdam.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pvgwvwpp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kikjjqrb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3abfkhrgn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3oiymbyyu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lktfqtaa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3acoqxhvb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xykmxeqz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nrzpkqxv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yeakwbcq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jhjlvlkp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bemwmxwi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lnduzqcy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ypbmlfmg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wtfznhje.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtvtuldi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jrsoqmln.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3welxqxfo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pihnwser.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3bgobbkvi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3qajjnvvm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3uooyachg.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3iqetckgx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pbthjkij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njwtjdks.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ksbjisij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slkhwyqh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dlxulgnr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3oxcaszyn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fbspabqo.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3keidkovd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3vfyuilsg.html


<!-- 参考信息 -->