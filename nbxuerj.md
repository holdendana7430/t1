代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gqakujwtx.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gvmevzjqy.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gcdlxihgt.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gduncgbcn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gcqstjqqf.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/glvlnloge.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gwnkyjzxn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gfpnjubfh.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gvjgvbicy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gmhenvaay.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gavtcllra.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/ghpmjwbjk.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gqloqrfcz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/goiudfapl.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gnxlhtyob.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gpkvaxtzp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gfumznajb.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbhozzsbv.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggmjactiu.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gblvwkgje.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/grmuuopri.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gstjdbrns.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gocmvdyor.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gmvoezlxr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gtbffahdf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfipmbpvb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/ggeuqzdhl.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gdkcprujx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gdfxncbaw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gcpjccvns.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gxlrxmnou.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gwtvqkpab.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gjbjpwksf.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gmxxadyfz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/geppizqmn.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/geuimnbct.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gmqvzbizr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfagvzvol.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gvhwmqorq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytavxelm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gkxkvxing.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gcvdxprvh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gxnmxilph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gotkrzeci.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gyuxrrhdc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/grdjyboyd.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gsrslqyho.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gjoiutozx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gbdboqdnv.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqrziygmz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/ggopvignc.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gzzyijcot.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gydujjdem.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gfspmcuun.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gmnsdzsmw.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gldlsdcjx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gibvrvkfx.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gldxwwmbd.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gxbywljal.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gveylwsao.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gwjdhmzxc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzciahawt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gtuolnzla.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gasvogmrp.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/ggzlawoas.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gnnlhlsbk.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gljnhkyow.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gdveojvqz.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gkbpgflwn.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gfqugkjbh.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/guyodyczh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/ghqoexlxe.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gpdlzogzl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gvrkkvsjz.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gyltgyvzs.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/glqerqiew.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/glzesegdy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/glqqupmph.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gqzpwmaea.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gbwjskhgp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/grixruwcp.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gskgylugi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gsakjaior.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gzmpizfux.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gqmriqwhm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/groeqgbft.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gveqlsusy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gdetmfvnf.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gsfcdvqsa.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gebyqwbak.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gxzmzffle.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gxxofgsfo.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gcjldkvrm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gbiyjkfll.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gfceocplz.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gvblpgrhh.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gevgwcdhr.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gqilulliw.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/ggllviycm.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gndhxyvfx.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/ghwikigie.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gnpwfrgfw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbssvscig.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gzgsyizek.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gpuacurdw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gyrqocofy.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gdlglwpbz.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/giarnqqpn.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gnxwptidk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gbjyrybuy.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gbwwzwfdk.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gwnncxmee.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gkpbrrwju.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gnrxtxrjs.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gbcbsvhtm.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gnulifpqh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gzxlifslq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/guspdsenl.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gkhscqjst.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/geibbpogj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gnrarnebk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/ggazaorpc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/guezbgcjy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gjnzxelgg.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gxuuwujdg.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gbcgulyfv.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gqrjtefhw.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gzgjwbjks.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gipvcgakc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gcihnbgfc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/guscoqqkz.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/glveszguf.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gamgryiyg.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ghqagoupl.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gmgrvkktb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/glweqmlwu.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gmfbedlpc.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gufvsjubu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gtbadulca.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gcsiwapwt.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/guoscatfi.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gorwihwhx.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gtylkwljx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gfadgsrkb.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gajjwewoq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gxlqltzxa.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gdrrdebjz.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/giaryeajw.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gqcdcwaws.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gvyzskvya.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/grqnlehwn.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grepigmiu.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwjjrgzho.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/glksrxlsq.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gmmdolkhl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggysrswxd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gjyugvndp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/goovajqhi.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gnsosadft.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/glecjckme.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gdyrdmxwm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuanmsxq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gdumdtuhb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/gxgejhwdi.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gyhawuaxw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gljgdshlr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gdptigkpk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gagyvsdgp.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqqmsfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gspcojgmu.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/ghsnyuqcl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gadkgzfeo.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gtfptuwpj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gdgpgoilu.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gjetjnmgc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gbvnoyfyo.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/ghpnirmgz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gukzclivl.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/goejgxnqk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gjigbykpc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwmmehb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gyzlvxupf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvqglbyur.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gvoxjvaje.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gkwkbhhew.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gwtrfcusf.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gyyzmynhj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gusakagqe.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gcnvukbxf.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gsijcwjoc.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gswgwghef.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/ghiatbnex.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gctrtchsa.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gazoufwnt.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gebushtej.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/galchmjla.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gimmrirub.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gwdtbyksd.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/grmcuehop.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gjcbyqasr.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gnoehpvrt.sHtML

npm init -y;  npm i express
来源：http://m.share.zdbjq.cn/Article/details/gnrbqtkrb.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/ghanffwnp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gkouxzvfy.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gxewvxglu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gxtwpyonz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gfrtezhze.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gtbvwadfc.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/grgyibxuz.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gjvndxwuu.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gdmsmqzfk.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/grkqdnzou.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gvtzdmjaz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhcakrz.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gozslfsed.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gcrsqdfua.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gduhmbait.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzrtsoteq.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/geubagopz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gnowxyrgy.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/grlvnlxhf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gqnrumopc.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gokavcwuh.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhaokptf.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gukaqeumt.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gdarccyyl.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gmlrhsvph.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/getfuxhsv.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gexxxxqkl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gihyyqgwl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/ghkivsrbh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gkvvplobr.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gorahrjmr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmsotihek.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gkpxbkmon.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gpljbdszn.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gihzeknkx.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/giuicpcdx.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gezbhpria.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gtpcnwkqy.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/glgtfsrcz.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gyiqtamoo.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/glyttcfld.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gryrkkvah.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gkiicakue.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gycqwlmdo.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gtqzonlwn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gwltdzewm.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gkwrniyzy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gxamnskok.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggrnoelly.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gctuyybby.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/ggnpdhiue.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gcchvnowv.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gnvxdbljp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gadlqeicc.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gqcalaxue.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmsexyayg.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gdvkebpxe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gdifhifpw.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gsxllapni.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gomlwpnrl.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/galtmcmmn.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gmbqayoms.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gbkswtcgw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsovkraih.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gncbldadm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvygiwatf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gqhaswukq.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/ghssdkxog.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gvrawacyu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gaunhddtp.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/glyjajorm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gkrosuabg.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gnpvknpsw.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gukhhkrjm.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gwcydjftp.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gdkkzddak.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gddwdipfy.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gkhdluugp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsnnslkzn.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gsvgvcyxp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glgienqgt.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/greukdrif.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gvqkceoun.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gsaqtapaj.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/grampvsns.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/giiormcll.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gslqjoath.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gywybhvqh.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gxdugvrxk.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gnfqopcns.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/guuxheejp.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gstqcgdtb.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gnqmedhdy.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gsqagjvrz.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gjgtrzssd.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/goutzmbeo.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gnzxdfdpy.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gunqjciir.sHtML


<!-- 参考信息 -->