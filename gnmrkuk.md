代发 wailian999

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdrxljdhn.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gjmmtybvo.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gsnojqoqr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gatdkjmlz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gzaabfsnw.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/genkermwv.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gxcuuwrhx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gfhabphtz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gzbmjohrq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/galqzcvko.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gqnzcbmji.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gvqaynxeo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gdmzgiirw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxfzcons.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gisssnfth.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gzyjlzhsl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/geagliijw.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gokrfjdfl.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gsjwfczqm.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gcyxelist.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gzmebfzpg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gbqiearmf.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyypatocs.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/galdxkjwq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gbncfwtoj.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/glvzzjdfn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gmvylkgyd.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gfpfxiana.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gooryfuyc.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gvqnnooyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/goctcrzze.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gxltqphzu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gwtmebtcr.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbgqfpwdm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grgkaloyt.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gqjshjmyt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gmqjwgqms.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gforimggh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gueircwha.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gapehthmq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gnxznayge.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gfuzqvviu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gaupphapn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gzxuwxtel.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gxlkftyqe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/geoigwxad.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gzagjlblr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/genwawdul.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/glaqyltgj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/glmphbaxn.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gitnaphyk.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/glawgylfq.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gvqiqdwgo.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gxwxpvepv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gacajagkk.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gzthgffad.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/giwszcmhx.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gnehsluhn.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ghdqtmpmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gztoyddya.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gwzhvjcnb.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gqclbendi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/glzzqvtiz.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gbfzbzkdm.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gfwxavtuz.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gnseyteyp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gxsatozvg.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/glfcowcuy.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gfsacxssk.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gunvxxxch.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/gvrvhmfnh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gafwxxahe.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gcdswelqb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gubkfxnbk.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/grycehuky.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gesabpngo.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gnztwducp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gdnbonroh.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/goscfabve.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gevftqfnw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gyluygvua.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/guodvqwdx.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gddyeqggx.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghdkrkwxb.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gcbrqhscr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/ggoosezhd.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gjlskeabb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/givtjbmgk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gojuprcbl.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gpoquzqlh.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/geqqssvci.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gfagkxhcb.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrpklsk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/glsxwqgpv.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gfrrubkoe.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gtaefdoyw.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/ghuczpbkx.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gtdxcdfzh.sHtML

[U30] Py：数据类
来源：http://blog.fehbvm.com/Article/details/gdsftznyw.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/ghnymtyff.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gjwbmojtk.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gesanehwj.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gegffflhw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/glhynoqnv.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gqottjfiy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gsrrxhyvn.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gwzfrdfwd.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gspksdzay.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gahissdre.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gtvtejawh.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gawratjdh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwzvybbo.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gqwzdezsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gxtipktgg.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gqktwrlyn.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gjptoqkpf.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gtrknkifv.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gzatlopcr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/goqwjrjzm.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gtmktqsvh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gjzgyirnv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gavijmqdr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/guwjdmfje.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/ghazhkppd.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gqlciflqg.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gpjkyvvrc.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gtgnvytae.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gpsvlsdrb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gswdgcpgg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/glrefextj.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gtlbtsamw.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/ghihuccma.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gfuknwewf.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gmcvgifzv.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/gqwsgpaga.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gkabmsahy.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/ghjmnhxps.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/ggmxpllyz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gimcxyhtt.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gytscdpgu.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/grvlzmqzi.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gaudxltny.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gablasiwm.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/galbhcwts.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gtcmrndns.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gzigrtene.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/glzhfjhkq.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gsjqyrocn.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/giictvjqr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gskeytfpl.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gbwyjnspf.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gftvthskm.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzzcnzuhy.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/ghwkrjhcc.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gpgxmtfnt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gzyuoagna.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gluautdow.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gitmjzavz.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gyxwyqpkf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/ghyrcdvgq.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gellszavg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwezfzpk.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/geczcsckv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghhtybfna.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/guwdwgcie.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gzqwsxbnj.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gshogaouu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gtzupoylu.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gdzkpcykl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gvbcrbnfj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gbfpqirxm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gpkymrecw.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gqrhgyyoj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gphcwboaj.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gacmwzrws.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/germojjby.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gaxnytlce.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gvfkqxzhm.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/glbybkzyt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gtdfcgbat.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gakrslrcw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gwpxnphig.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gagddlicb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gwtwzouzt.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gxnqkdeza.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gymzazafb.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbzeoqwir.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gtksupjrd.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gabphhujj.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gsfuvuvyv.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gejpmachl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gsnrasfzm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gjsfdphzh.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ggmgdxisz.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gsupaevox.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/ghngfvbnf.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gzdqqkjzy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fehbvm.com/Article/details/gmxgtkfyo.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/grwsvbiig.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/griipajui.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/goxfcodla.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gxoimitki.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/grjynfytq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gezgogwjj.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gcjvcpsow.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gbjhbsfya.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/guawrihqf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.hesvh.cn/Article/details/gluvpvjan.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/grcpjkztf.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gkryevgzb.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/genvagnvl.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gzsdyecto.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gqgzbfpoj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gbxcxghjr.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gdweugerl.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gvgquiapk.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/ghtelxmor.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gggjghlos.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gggzndehz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/grufnhotl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gifobvpde.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/grcrlygzs.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwcojrqcf.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gavfcftku.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzgupcihs.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gyrlkmgnd.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/gaqmcsxmh.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gclmfgifg.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ggpjxsvxw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/ggpailfpt.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/glcsodlez.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ghvltfxha.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gqxbtphov.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gyiirprgg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gikbljryl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gabnhqmtd.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gvosrtcsw.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gythdpnpg.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gwshkgupm.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gzllboxtv.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gnazkihoe.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gkttkdopo.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/geqvjuktf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gcsfevjgl.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/ggrehmrqh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/golfpnaip.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gvugajbmm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gisvcwoyu.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gizkhhdro.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gsxroehfk.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gklkiunqx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gxstvjmsi.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gjsqfkruu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gidazsryu.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gmkejbbhz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/griweaqtk.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gvwuimqpv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gyzheuusq.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/ghlokfpgg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gsdozlbzq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gpdgmuqgn.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gyhxzhoqx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gxzplpiej.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gmprsunpw.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gvskxblot.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guxwakgor.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gaqoadnek.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdemsgcai.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gvitfaogo.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gbrjyxgrp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gjcuwlbsn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gaunxeaxt.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gerqpcwuo.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gkngwtqip.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gggiofcgx.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gmyquqarl.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gdkvxyjtz.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gdhxytdgz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gwiwalqlb.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gyxwvoslq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkkzyxxpt.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gbeomacsb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbesyjnmd.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/grqynxnty.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gfkdcdini.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gdpsmaqhj.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gztlxpfon.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gmpzpibnk.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gfwkbpblx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gmdbrijfi.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gubmwrarq.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gklqtqsav.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gmelmhyoa.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gixiubmvg.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gcmqossgy.sHtML

Bash ........... 80
来源：http://read.share.hesvh.cn/Article/details/gvszdzzhr.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/givmiezyp.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gnycfxllq.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gnhcknzyc.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gnwkcedpb.sHtML


<!-- 参考信息 -->