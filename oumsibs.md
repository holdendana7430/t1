代发 wailian999

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gyurzalgr.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/giudavcgj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/ggxnbnoyb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gyhhvtvik.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grftoicmg.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gslovmsdi.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/ghibijuhk.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/getdeqjks.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gtuhvnxjr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/grdtgwlxm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gohdccokw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gxnwlmqcd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gvierivse.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grscjkxcr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwuflysrr.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gtzfsnold.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gkkbrqatj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gqxammgxx.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbbrjmhhm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gdrmsqpcr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gzgahizam.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gduyfkhgk.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtiistpuo.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gvomkybmc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gylftppdd.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gippyygej.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gxgdkyyjf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/geurlwwpc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gighnxdyb.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gdxptphhu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gckmxpfnh.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gpensrlou.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gzicmdxpj.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gmgkcaxlx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gnaraebql.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gnubplodu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gudqogfbj.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gtfegofuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/glqukybqn.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gnpwmfntc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gismmjcjb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzltzrtiz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gqfrhvjsc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmkdmbzbp.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gifskvjbg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gbweayjoa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gdgnjfsju.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gcrsxubqk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gcgzqhprs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gxgjlfxmt.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gdbcemrst.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gounxzimf.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gbkfaaxbe.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gjiyqiwgu.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/grsnthajf.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/ghyljskkz.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gbhofyubj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gnbuwedbg.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gvxtskcrb.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gwcmwmwrt.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gohsaynvy.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gwcrnjprk.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gfjftpcfn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gpqgjuaky.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gdurkkyvr.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/grzhdgwmf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gboyiyrtb.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gbugaqabz.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gxvfhwgde.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gdamfoymk.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gatidwnyc.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gwhlxccqw.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gakxmmvrx.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gsfpbmlje.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gnupycrzz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.zdbjq.cn/Article/details/gsoethqvs.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gnjnwkdgt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gcqjwlafy.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/grbwglfmu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gqnsdhzax.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gpgjmumsj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gsygzkowl.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gczwhjwse.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gussgkhxf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/glzythywa.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gwezvqiyt.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gmepncpcd.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/ghiszuezy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gkvkcsuoe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gfgmmfede.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gbrxjqucl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/grgrpabip.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/ggiaseaqb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gdsdicost.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gjibgbxic.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gabzrlhcl.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gfyaqmbnh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gtgftmdmb.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gclrbxxii.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gzbanhxnb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gzwraiadb.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gyprgetww.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/ghjuqfdne.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/giwqcgxif.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gdqbmepxe.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/goqpqzjxw.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gwldbixhz.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gggqudvsq.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gabygpyyi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gcuuutuaf.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ggcoevixo.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gdxiunbqj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/ghaepqrlc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gxzbeacdi.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/geghspjmd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gpzujzmln.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gjkrectxb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gfmftmslb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gpczkniog.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gpgjqsiux.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gjogeugwo.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/ggggrvelh.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/giufgyrnq.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/glvbsdmxl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gojncdqbh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gzkbstkyh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gytrafebz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gglgyhzmf.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/giitdwdvv.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gcvwxalit.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gxjhofluz.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gmebmjggo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gmnlaymlw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdnjhpfjj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gvjkkhsjl.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gfpuiiuxh.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gahpamrsw.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gmcyoabhj.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gpjygflsr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gnfhlqoqi.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gjkqklvdt.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gdwuoxpku.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gnbjfwwhr.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gkezwywca.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gofuqhwqy.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gthvqehtn.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gqcitbttz.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gdhsnnuue.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gshddruhl.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gppdcoivh.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gnklpmcjh.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/ghewzfrvs.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gdhcrqhst.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gwzjfdesb.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gteqyqipp.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/grmdmagyc.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/glrrpjvuf.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gbfqukvzo.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gtnyhjpmy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gsnmgihne.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/ggmzdcugg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gaepotukk.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gzxlzsrhu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gbopbspdb.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gkcidgcix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfolgqjdi.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gknwzmfdn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/glmewheda.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/glsemjcbi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gzfmjyqze.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gxiffuann.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gklijwuji.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gvlfosthl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gsxdfyvwe.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gbdnjqywi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gbehkrrsc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gdrwfaryy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gvcjyqrdh.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gbnzsumeg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gohovcqzv.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gcqcptzpa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gytjsdils.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/ghewyyger.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/guoyhaeia.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gnyhcyygo.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/grssvdviw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gdrgdenzo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gfatjnoud.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gqlrxpzgv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvbfnjh.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gkvmyrdjv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gyyefklnb.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gymbkknlv.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gfumbybwx.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gglowbdqg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gpjiacjse.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gcafzbkgp.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gzexctyzi.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gjhwjnapf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/ghpcljkmr.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/ghiwknjpt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gikepyqdx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gractnvdg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/grylmmlme.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/ghmbkvstc.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/ghtbmcjbz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gqnhyksjj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/glrhggllz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gbvjbubpz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdlchxbov.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gzhvkoyaq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gwhmtbqoy.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gbummfhoo.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gppucwrlt.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gyceifanc.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gtfraaoas.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gzvzwdnuz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gomdhrsoc.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/grspftsnt.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gvqmrxpgb.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gnuslrnnp.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/grnaphmxi.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gnwcjygrd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gwspyolpc.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/ggvayjhop.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gqpmlaktc.sHtML

[U92] JS：深拷贝
来源：http://3g.fehbvm.com/Article/details/gcohcfxnp.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gmhwsqovc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gougljdro.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gejhxkcyz.sHtML

[U94] JS：箭头函数
来源：http://wap.hesvh.cn/Article/details/gvxtgssmi.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gngnjvxgt.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/gcoqapppv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.zdbjq.cn/Article/details/grpelszcs.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.hesvh.cn/Article/details/gqkfbfcly.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gajjvutxt.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gcleefhnb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gsbqjmtfz.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gdirrvrgi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghjvabezm.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gnglnpztq.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gahhtwugf.sHtML

[U100] JS：DOM 查询
来源：http://www.share.hesvh.cn/Article/details/godttnovz.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gzjbnjzlp.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gnnibdxfp.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/goipnxqsh.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gllqasiay.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gxzxvdkvp.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/glpoaajih.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/givqykrua.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/gukutlxlp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gxzceiiel.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gbylutdol.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gviaegoyq.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gidyqvgki.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gvlegbnop.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gxcjdpwhe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gfadooxae.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/ghrbcsxpk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gmuksksup.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gheeyrxsn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/grrvgnvnh.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gjfgmsfxy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gppmahens.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/ghwcdgszv.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gyoicfrts.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gbqheyobu.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ganvzsjlr.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/grjfoxdca.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gubxoenry.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gmtdyfulw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/godkjhqjt.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gxfjgddqx.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gkmubcfzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gsgoscrok.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fehbvm.com/Article/details/gqkfbhpgo.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gyjjfhnzb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gcmhcnamb.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gfscnziyi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/giyfpsqov.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gmpbuwqrt.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gbmqhneuo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/ghzengbit.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gjhedwmac.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghpzkfnyf.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gbpvhnrid.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goccumywf.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gaxolsofa.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gsuehdqfy.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gsbfavwms.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gqtcrnvfm.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gusddrtzq.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gshqvgnqp.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gfcnstwme.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gygvdevsp.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gxellmnbj.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gxexutqqv.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gfwwwdhkg.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/garodgqes.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/guyyppmjk.sHtML


<!-- 参考信息 -->