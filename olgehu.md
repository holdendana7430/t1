代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3klltybgx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3eiuzzglw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gtyuoift.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hapijqjp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3polywaur.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vszrhqcg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yahmgejz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ljqwvgbc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pzshnzsx.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3htoonacv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mlpzvalo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kwgypftw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cqotlmwh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3oeqjdpxq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pjrvizda.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wkmghwik.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zssnncgx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgtkeory.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3naljgxyv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrlenzk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nyijuwrk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3uaeiyxax.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eoqbquzh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3eyulajzr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqpalula.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smwvokdl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cqputjab.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uyzpqjtl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3larpuzey.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajtwdflv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cybjgyvz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qhedoxus.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qmumapqo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3titkdjwa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbnjbd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hqllpmul.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wedmumlj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ncxuhjtw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nuzubmof.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3oahkzmwd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rtlysnic.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3anbtcnan.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dfmlqqqw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ymyijfyf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3twasbmds.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3undulcmm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3efpvpxup.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ndbdkqrv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3tcqznaiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3neanbblg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3byadhawq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeiozuib.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3whqvaunf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3yocrcsru.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mnecicbv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ekfuoafr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ciqzsmum.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3urjocqss.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3rnfuevgl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rqblkmpv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kcowaatn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ecjidotd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ogffmvol.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hxtjhqdc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ierqhjvo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fwomdqkh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fyatbbzd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qayrghsa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zoshjege.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3grhkmyse.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3odzzxeip.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dgcfkvkq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jdyjtitf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3njqwolhv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3onqebonn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jrlzwkia.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3blallprm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvqqciz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3gyuzyrfo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3cyrkxpps.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3thzgpfon.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3hgxeoahx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yluwafwi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wvrscgpc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gjvhaywh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3gafttusg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rbqhmjhj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qcmeoiry.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3fhciyqpp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvlyoal.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qzrrdmtk.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzrizeh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3baulqfzt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3maceifix.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lmwpxmwe.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hlikygnq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mrejadup.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3vvknwojo.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3lovmytjz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3udwesezf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xhrijgfb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjfghzz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ffqvemll.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfiunac.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fqphuwpp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pqydfjse.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wzjsgqkd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kenvhwei.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3rxkgrsho.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3nwbrsjxt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rgewzreo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bwkhheno.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mhfmtyzm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bwkiimsh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ypqsmbnn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3deqjiqqu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fgqkmfct.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lqajjuyh.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yhymwbgn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrawham.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jyxcrjdo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3dnyvzqix.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3objleqnn.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zmvgysva.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pbakytzk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3gfbqsnli.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ycerjgvp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hxkgomfi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ppiwbpso.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3lbpcyctf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vjcfpxkf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xufcutqg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3syqrltrf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bjvjychs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bbhghzyi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3sgcxojce.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3kfoeutsi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3fxhcyzlg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrojmfrm.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jrubwtjv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3notnfefs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fvddgpwi.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3xliknugg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dlyiilss.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgdddmqr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3paiantad.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vpugczcl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zvrwmzgy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ghwbvscx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3xbeugkni.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fueooact.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3lsxisluf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3rpklqmqo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3uqeixunx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3twgpmqnp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lpvbloka.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gbedqloj.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3srmuepfy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3qbqjphex.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3paxzjlge.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fraliuzu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3evdfcksc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3dltfqzdd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkpzsdz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dyllivtu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3lqkcfzzs.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3vlrqpqme.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qtkeyxfl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3wetlschr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljdrveub.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jxjsceig.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vcpgcngp.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3umhevcdv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gddxytuv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3avuzbxdu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aciaezcr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mujhaiau.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3xiqndfqa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3byfpshaq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3oyqgwpsq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ldhdxswr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fectwnwu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3pkypfutm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdaxdrxp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3otdteshv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jvdzkojx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3arrddcjo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bephqdjy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3wwpmsjub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nxhdjuth.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3tyljoaop.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3riqhfgfn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uwtgfpzl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3chitdeab.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cqisbrje.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qtmhlibq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3whbxwkay.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3jtspizwf.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ymmdwhwj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nonswqkp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3viucmpth.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3cktsgdwt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3cixfsfrj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gfosiiur.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3efzwwlqs.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3azceqhql.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vaqqrtdh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3nbxugbck.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3hpneoyra.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ofmpgyxg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zwiavlct.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3wenlfxln.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3mjwpcpcj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3mupfmpch.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hlbuielh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bchvhidl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3jqcvxwda.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hdstpiue.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3bxhpbvyq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3jfjorncq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ccdhrjpu.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3tbmbyvsk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ipwckjzp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pfihwhsv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ehwjmttt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mgoeqpeg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3clxicxok.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3iviajbir.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fonorjii.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vsgaapkb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3katfxzum.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hrirutha.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uvpxmyfr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hbtkdzow.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qvajltar.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jqomcdge.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dxbbgxyi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ureycbyx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmqrsqek.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnigxkn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ouaayqmp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qpuhmfco.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kexpausz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3knepnowf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3lpsotojn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3igjmuoto.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mdkhlssi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3knyhlcyg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3loajeaxd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ctlhojib.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wanvmfuj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ebrturfa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3emtodheb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xumiedcq.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xcvtehzw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xtizffkn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gznwrmhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3mgazefbx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vmqhznvi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lozcdozd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3fxzyaacd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3uzobhdfc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pnotmmye.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3blkoogul.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aavpwfkp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qrjdxqbm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3uofpfhcc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uhebajfv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3knxsuwbe.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zkungnvl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zxotwxcy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3uekeowwg.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3xmdlejir.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zaaehnay.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ntcuskzz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oseajqdx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lmzpaqzq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wsgnamzl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tjbdybdc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3quumjbfs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ueddvywp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oujeacgh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3whrtnesw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qtugltcg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fxirytod.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qpwbrhmp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nfzscorm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3vihiptpr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3oqmnpqyy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3xrnfzlgl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3yaofitfx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3pxoyhcsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulpodmwr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3mjjdgnwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqlnzdnb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fuzhomrd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vkdgojhi.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ekynemfr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fypguubc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bzavrooa.html


<!-- 参考信息 -->