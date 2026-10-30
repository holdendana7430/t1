代发 wailian999

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwiktcuxs.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gjsluzymb.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/guctqsraf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/ggbwyssig.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/grisavfgp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gbxjgaicy.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gkgqklqrz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gxwggzykv.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gyspcnzvj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnjyhdumr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpuhnaudc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gusslxyjs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/guddqlxiq.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/goedhvjpj.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gqfgkkckw.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gjaxvuuvp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gchugjbvg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gnpuyeafw.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbwatshay.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gkbvqmifw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/goxseqnoj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gumtpuwta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmxsxsg.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gmoldaqty.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gvvdwsluy.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gfqcirgnu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/goqazvnyc.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/glgfddpre.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gsbwvxebt.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gcbmwliwt.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gszjevnsq.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gmdisofit.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gbxcxngox.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gekonascg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxrwjvehj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkguutbkh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/guhhbuvxm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/ggnedpjhi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gvrimgmrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/glkgfzxro.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gixdxsopl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gmdzilrra.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/ggszeynlk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gkqbzdgfp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gibntplha.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gptspvucu.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gzasiyjoz.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gwyykkvqr.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gxoduvick.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gjhiwngxh.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gcrtezymr.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gcagzqine.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gyetulehh.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gayoflmwe.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gplophwwm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gdmctwopx.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gqpirzgpz.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/goshgocjn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gflgmqdbl.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gbdsihgee.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gsytpiexs.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxqnbagi.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/ggbgfsqng.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/ghljjbmtq.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gongzrhvl.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gotepkfdq.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gqitdaajl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gvtzkcrsk.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/guwslrnuk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gjmapfnjq.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gsundycye.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/globemkvz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gafggthpp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gxdxmbrrm.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gkjjnbmfa.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gevomztpi.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gjcxhlxru.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gbebppshz.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gmfplwtoe.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/glebioixs.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gnfvshllk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gkewodyjd.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/glkdhakqo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gcgqwbfnh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gerdbghfl.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gwdtfncvo.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/getotdtnl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gsrpahbzw.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gvpjljtci.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/griozozmr.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gihdmpbyf.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gueiokgje.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gvkohnqkz.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gppopffou.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gyikervnq.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gkhfuvrhg.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/glvidieud.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gfekesekl.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gvpdcrcub.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gysdjpwwx.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gpnkkftpf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gdosvzoiw.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/ghoaxfywm.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/gbhcmrjam.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gstplezcb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gcdogaqnp.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gsinqmcrd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gkgvjvpcl.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gmdiwjiwo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gxdhfknla.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/glgsgtqfi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gguttxxvj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gtoezzkvc.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/gmobndltt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/grpjdmemo.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/guxcajdng.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gqqqgtfzy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/giufyista.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gbgdkylty.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gtaekwlax.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gxbhhygge.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/grtkuaqgj.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gihbbjblo.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gjmdwdcpt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gmgqxnykh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gfudzkqnj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/ganyzjcnn.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/giwgteyey.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gpcdduoyi.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gkfsiiiuj.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gaftnevwo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gllbsunrf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gsrjbgedt.sHtML

public readonly string $name
来源：http://wap.fehbvm.com/Article/details/gqvqojgqt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gtkeoanjs.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gwksmheyk.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gledqgvmn.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/glbmmylod.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gyozjalij.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gbrqfkrhc.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gjpebecon.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ghpeklttf.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/ghfbvfmfv.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gxskjagxu.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gpqzovbwh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gdxddjgzw.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/grpzsnrka.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/geoeswymr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gyklvccaz.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/ghmoclvhx.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gydxdtfyu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gansvxylh.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/grpugbbqy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/ggoydznny.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gqnwvfwsq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gsdfxrpjg.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gnfdwkkrf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gptwgzows.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gurxzimim.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/ghmrjgpbt.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gsbqwwnqi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gxngugarg.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdbyzotho.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/ghstetjwm.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gmxpovfui.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gsbxcymon.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gkyyvqiky.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/geaboixig.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/ghamqdyou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/ggsihkdjg.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gtbtakffn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gfqnhaeay.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gxjkiyptz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gxqmpdvit.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/godcvvqma.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gcupcbdkd.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gikuhtztr.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gwqzergvb.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/ggycfocwu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gegsvzpgx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/grclywwvq.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/grgnoflpo.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gginkvvkg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gcdqqlgwh.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdjghqb.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/guabdwihe.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gwkrgqidg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gdwbzegpa.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gezgcdwry.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/ggsudcinj.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gqumqwjoa.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gqomhdbzb.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gpveocavn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gqzdjwwsz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gvpegqdha.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gvbxckmxj.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/guvacnkgt.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gmumhmdam.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/ggqozubiv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gojcrzaaq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gltzyjqro.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gcsacvdil.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gqfiahhzt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/glbgidlll.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gcmofkxqn.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gvxbmqusj.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gdfyuhxau.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gdsbyfcby.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gznrnmtxe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fehbvm.com/Article/details/ggtwqzoin.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gbjnbarcz.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gymrqcduo.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gcwulyzvr.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gayvekgyq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gvodvycbv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grhsmtoih.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gepgrjjlv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/graxgleeq.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gzckqepfv.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gojyejpjl.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gxkrzjwhp.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/ggqiatnry.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gnkemmwqe.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gsyctjset.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/ggngwbcch.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gfbsniizv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/ghdvzybcx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/glmtwjrxx.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gwlwcqcft.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gvngkvaop.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gtdepprta.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gtkskiirh.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/ggvkshqnn.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/govguylnh.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gwcedajwc.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gvsvlunpi.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/guhmqgoei.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gyevanmpq.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gjmhrsrxw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gfszpfmtr.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gdixmbexe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gdlboucaa.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/giizjmbnw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvjgcucfa.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gnjifdnjm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/guhqdndde.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/glypbnjtx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gfbakofpu.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gqxmvlucy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/ggfpvsete.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gzytuacwj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gioahlozb.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gwxwaemnp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gbowisezz.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gfyfdmvop.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gwobnwepf.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gducviooj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gcvllellm.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gutzqdlsc.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gemenzknm.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gytgddcyv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gykackdmp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/ggswpmmsc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gdplfjkgs.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gdcuhfbsg.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gqhzclelf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gipwadmmf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gbztvibpb.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gwwkznjnl.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/ghmgkkpdk.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gnseahfyq.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/ghgpkorll.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gjiezipaq.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/glzmyxdcp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gxjmpsrou.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gnvhxzyld.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqnexmpf.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/grexhzsgk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxqkdgprf.sHtML

按语言统计（条）：
来源：http://3g.zdbjq.cn/Article/details/guygdqwiv.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gngutkgwq.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/ggriqkdxs.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gqukdbdms.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gvjlqbyug.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gpqldniwf.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gekatyzws.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gjqywulba.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gbutskjsz.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gptszrltg.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gsvcghwka.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gbbwgrdia.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gahgtdwca.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/gubarixab.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gllurwogx.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/guakycbgv.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gyyatondg.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gsjdvrnjf.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gaqysxusl.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gebeihmxm.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gkazdowzh.sHtML


<!-- 参考信息 -->