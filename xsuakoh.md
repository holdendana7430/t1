代发 wailian999

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/guygzjfkk.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gfcmsymwm.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gobbajosa.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gxudysnyl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gyyidvunr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gqmodkkxh.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gmpnptjpa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gohowijfs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gnsikworh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gusbsfvvj.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/giersxyun.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gdvuymmit.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gwmuvmtva.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsaifzivt.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/grkdutxnp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gjfhfqkgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gompnyedq.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gygsvtjem.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqvgcthys.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gyssxpnrj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gbhygwgjj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gjixpiriy.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gohawecpe.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdacvrbhq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gterqiezu.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gzszumoxq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbwmrfve.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/guhlqyacw.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/geuoltaum.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gijhzhojg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gpvtfdanb.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gnvxfvbus.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gvmtrhmoi.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gwceblqai.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gwzpsnzhx.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gpewpkwyc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gaqvsuhwt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwuvicflw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gataxplzs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqykyvjhv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gcttpzmko.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/geiynqorb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gpivleisz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gwqhtqbtj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gvctextqw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gdctzqvzc.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gbfifwbeu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gubkbuinv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gbzzsthgn.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gcqlhhzlx.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/ghyhkkmpq.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gzrgrysou.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/ghylywtvw.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gpahmbpzg.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gtnvuxjzz.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gfkqijkii.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gkjajypts.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/grpctstss.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/glqxivdpj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/girywcbpv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grfepigto.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gtqqdacss.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gxhlimdai.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gevlyikgl.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/grmoxnmlr.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gituoszsd.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gmvsfzqxj.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gqpilgiqd.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/goswyzshs.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gvipgrohf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gulvkpnka.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gxipmfhto.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gzkcwidpg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gmlavjhnl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/grycfgjgb.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gdswsvicw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gyynccsma.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gadlfqnil.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gmlypqhgx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/ggjelniko.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/geewegyia.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gtzajfndj.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gqxhxyszb.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghapsdwgq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gfrrbnyrq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gdnrhrbxe.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/geyxidnnm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gpdzrvbmn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/giztwwzcc.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gvpktsgxh.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gqyjcfhlm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gxmwblrib.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/ggzjahzld.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gdxolnkgs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gcsdfubdh.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gmoqlyfxk.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gjooymbni.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gbojxdcsz.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gdlwlclil.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gxhupfwzy.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gphzhzgfp.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gvujhqkte.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gkljpujbe.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gebukukmg.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gpsnkltee.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gfgqobtdc.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gmqvizpcy.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gorfyhufq.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/grlysihzz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyanjzsc.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gisvfofqv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gxqchjijj.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gcofdzkjw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gpakkpxgn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gtzszfqnr.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gcwtqdppz.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gxgxjwhrf.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gueuvgsge.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/ggsoljxzp.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gvpscgshk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/ghrhvhwnt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gbsbzyitz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gxxpawcsj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/gkgwqpwut.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gsvtijxwh.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gmorbqyje.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gpftgywdm.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/giataaydu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gmtnpixrl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtcrkbqtf.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gcmwouhaj.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gtbxbflhe.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gvgxbyrdc.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gjqwikymx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gsqncpsxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/guoyrgviz.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gvvylhvbq.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gtwnmtjhr.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/grpbhwpgk.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/ghealbxgu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gojqrtlsx.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gnslpkvus.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gxjkxroqk.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gemgakjhe.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/ghdfrbibs.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gznpaovyq.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gidpgfvxh.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gnbpvjmsz.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gapkavdej.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gzytjyxxy.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gzlidewwu.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gobdajfdh.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcfxfsmmg.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gyphhytyj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gyqnrflut.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gopqilazq.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gzxjjapip.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjiqneoyj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gyiqoemwn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gfmtmztjy.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gbrjxxdnu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gccxnlldx.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gfoudakwi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/guphnpfau.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gbpwgpgju.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gjdeuzroz.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gtexfkibq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gijectkmp.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/grfghshpz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsrywlhfm.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gtusukwef.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gwrovyimi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gpwtluugl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/girbsrycz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/glqagmpss.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gezonzwps.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fehbvm.com/Article/details/gqdzbftqj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gtjdvdeqs.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gqengbmtc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gwtwgyhvm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/glbqaksiy.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gidpxbawl.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gpmvmcqwz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gpyscxxsb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gxyquawia.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gcnyircwr.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gmherfeue.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/ggzyrayhv.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/geceztcdx.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gwfjvhcbr.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/geiuwyasb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gepakydms.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gpkdwleni.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/goraesxsp.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gmqsrcozd.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gjqsngmsu.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/giqwrxbct.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/grtldviks.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gkloedbrp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gcfumlqso.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gzcehwgws.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gwafjybwe.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/gqwapafur.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/gltosozfg.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/grxatpbrs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gcyphrrhm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/ghpujublz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/goujshdam.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gcdkflner.sHtML

a?.b?.c
来源：http://www.share.zdbjq.cn/Article/details/gdznnmcxr.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gtgtzkgio.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gnmofejae.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/guvjkdmrt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gkmizztcs.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.zdbjq.cn/Article/details/gvvdgumqx.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gmnrihhsc.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/gavcpkkqx.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gmpfzxfxv.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnxgxnzjd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gywhvnlsz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/grpyhnuwu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gmdkunksw.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gcvysqtfl.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gmhxalwyd.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gyjyrwwjg.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gtmbolxqt.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gvklbpjrv.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxpboamte.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/gduxhyoyv.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/grmomuypb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gsxnztbrx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gbjhofwcw.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/guxffxghs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grhbqlxmy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gkktxcffe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gloxohava.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gjvmsszft.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gvukrburr.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gwzrtmzya.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/grzjixaau.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gwjcrnzmg.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/ggpvenxqt.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gjkahzems.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gmzjmmxym.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gopmeedfj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gnwqucweg.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gnfyyejje.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gwmwiywbi.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gohaluebk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gqexllzsx.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gcvqnbovw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gznqbfqwm.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gtjorhnox.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/geqrihdza.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gxdgztkda.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gmpggemnx.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/geuklupoj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gpmcjygzk.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gjkextthx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/gassoguiw.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gzgngmncs.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gjljtybfu.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gkmgtxdcn.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/ghswncuma.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gasqnswjk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gemlkmkzd.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gpfzykwpx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gtdyojtim.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gebiccruq.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnjmxfo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/ggbzsfpuy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gxwjnrseb.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gmmlzbbuo.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/glogpbnvp.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdfepczmr.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gjylaajgy.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gxivoxlpy.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/ghbeokvdy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/ggasfawfn.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gujtjeato.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnkofmtdv.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/goknkcvjj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gptluggze.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/ggqsqkush.sHtML

Python ......... 252
来源：http://read.share.hesvh.cn/Article/details/gxvieayhz.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/gqvpdlqlb.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gkffoabup.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/guvmbhacy.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/ggqmxwrax.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gcnnlovzj.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gwhonzxbc.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gzagftidz.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/ghhfatleg.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gpxarkihi.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gepybjssi.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gdpjxivos.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gwweyrgjj.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gqgscnnlv.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxgmqiy.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gkswoolhn.sHtML


<!-- 参考信息 -->