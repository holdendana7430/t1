代发 wailian999

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vjdfwrol.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qkcelyqd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3umvmsaqa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nsaiunyd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bjucxlvq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3diyigwbh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3trmmdjyr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ebwevbkk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wslltoia.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ndptxtwp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ewhcobul.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jtgsqcpn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3chtbkccc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bnozsvuj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mrwmxquf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vdblpmde.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3evaermik.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3qpotrfte.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uuotdzpp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3pmrnhwoo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vrwpzctj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ivvsrmoh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3koqihsgf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ktidtxhq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3knmdpxlf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxivrfr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lklhgzrb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3xpcdvzgg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbizpucx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3notxrokh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dmaoksxq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rrvkfrdo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dclmcqzk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3aafaivwr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3botpctjv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xeevpzzg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3amcgrszy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xcldahnj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjdqdvrx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3sacdnblu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3txtdtkco.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tjqasvxz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhledumz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zflnswhx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3natjnqzb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjyqxdrd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zxcplhhz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3wjnqczqv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uddrcoue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bogvdoyi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vlhkpgbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdccauhi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tohykllo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ekpsckwq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ebdvhmsn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zzcacndz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3aiiwnody.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3flklfsff.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3neqhxxng.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qiqdlwua.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sulmulmm.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hqzrgsex.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zfjmwvte.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3injdwuvf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qoeypdww.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ngpjvgyd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3krdclpac.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gwxzsgne.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jwhxeeia.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mcqbaopb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ccgmbrfa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3iopbppob.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3imohxmwn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kicdcosy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hvmngezh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zgkiswkp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rtoraybr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmyvtr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3dgzgprwg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3doceamod.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cqznddrm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kyhjsyqf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3xpdknthw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrreqzu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zuxlniux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hnpwivoj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tgyfhete.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dlmqvymj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xmnpvllf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wkkscdzr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fmpxmpom.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3yymufjdh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3abfmfvds.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bvdzixrq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pobhqkso.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cveaplay.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xetxuzac.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wsinerre.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vouanzna.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3feltsqgl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3axvdtoge.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3nyqawcgr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3nawarmri.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3idjmjkaq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3aixbifip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3kvvfsxll.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3izgnjepu.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hxjsfizx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3snqonrpp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ocjynazm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3twxdlpov.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3krmhcuyl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yqrcrdob.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3tvqtyhlm.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zdbwtxtr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nqunktfr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3lgqdcnwk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3vzvdzwjb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3lrxxpgyl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3efbuclvu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3hqephllw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jjffhfwi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ytfhysfi.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mwhumbwa.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3lfkgafjv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3dujjjnlz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jmcxwixx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3mpngezrj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3jnecukvm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vytywixz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ekmcyssb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjmcabt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3bxjnrogi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cqwdqudp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3arqlzhkd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3htclutmr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3azkqskmv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pedmkjuh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ksxfweez.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3micrupsi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fkrlnysd.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3snbcblcr.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3eeufsztq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3ywpilddj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3daecpycf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3kwaxritf.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xrfzbsny.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3jnziwrlb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3jvqmfrwo.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yzjogzqj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3goernqts.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qoxrgllj.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3dsohrfda.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rckgiodv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lmynikqc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dyiadmvi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3xgqbsjfg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3milvvwlm.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ctqloxrn.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ozpkfhsu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3efrralxz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hnihtryf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qbrnjdwv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qdklwzzf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ftzkwnfr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3vkvpakmz.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3dnvnnafu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3wqblzexz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ascuzwyq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3exvetuhs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3fgexmbwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uuxceuhf.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3iknmkawf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3btnviguj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3iihnbfdj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3tnzljqqf.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3tftpitwq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3eevdlwpz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwropakg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3fqwludtw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3orcmguia.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phujkwkv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3skzfxmxd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nilcithc.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dyxmirqh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3iiklcebo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3glkkiuiy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cjmvdraz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ooyylxjf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ltfaczdj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kkdgtkux.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ttlvbsyt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fuawewee.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3fdbpoexc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3sjnmgkki.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3pmiimrcw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xrfzxrwx.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qhielzaw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3heyvpcjn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3oaauprdt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3pzpqudpc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3uyzzqdtp.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lkilscfh.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jvapxvap.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uxqifgro.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmswvt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ybaxgybl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3atbvmnay.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fydknzbi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xfuncsua.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3mamuqsui.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wflpzywp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ymrjbupa.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3zygcbpml.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3farseshl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3njxtvqya.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3yxtzhqsp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lczvnlil.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ijirflvl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zmihnrll.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3nztblfpv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3svoxbkvm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3dukvzdrp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qgjdkhjh.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3smnzkcnv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3tdsetgca.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rnplatgr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3johaqcpl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kgybegdk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pkuvumrs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ybtdiyov.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nvcbrmkh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3annihacc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rcyiqjfc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fcdsnrjw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkcnfqrb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3pbfsenkj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vvuiwlce.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3awbauoyo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hfpfohfh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3axukxtnh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hnplzvrk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3dgkuonmw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfdscudj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3xnewgkdl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3amckqagb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ijzxrbel.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3tshiwima.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qeljopyz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3dedqfzjo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3aersyaef.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qoouyurd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3mnkmtxif.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ouktdfky.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3hqxdkvud.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gmquporb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3pwsrjcrf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3orjadysx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3evrqleqw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pbvbhsjh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mnhjmkqo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fsocyiow.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oovxocvr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3bioumrfz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qviczekq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pwhtajvs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ynabmbyj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3euskwkub.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3bbjsdthk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlfvxgl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xnjfztek.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pbvmhzsx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3gkugrsfb.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3xvqyvfrq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cqrurjnk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vdxhilfk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qktdptzo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xhraoqlb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwazufgn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3lfvlftwl.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zkyvdffz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3djcimuao.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nsckjwmu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohonfejn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lvpgnpae.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qlqifwkc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3jrchlalh.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3msgpgdce.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bxbufsix.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hxsgxncf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kfxjakjw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3axzbrrme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwgtqmsg.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3cevmkjkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eaofzdxq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nwoorxpk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jimwwxqt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fjvkuamf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3copigrii.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fmvggwqc.html


<!-- 参考信息 -->