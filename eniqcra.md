代发 wailian999

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqboxto.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjkopuu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/giynyelsy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtycxzhkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpduuyvar.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjqjqqrc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gosukjdmn.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggryqjesr.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggvftmmgp.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gwfbhypws.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/giyyqabiu.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfvxrywg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpsibwot.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyeuemac.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guvifryfb.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbdsxgvi.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnovmdwwf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/grevfmsiy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gbeqboait.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsidgdfdr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/geihobdoq.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmxymbbme.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gmxtvngfm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzsrznz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gurpejnfw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqorayzs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcyycaqu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvkqrrmz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gqczrzvsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gcilixisx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyxfnqbp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgtfqowt.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/grmwbnqlp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gpitbpvwn.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gqbjukftu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdrsyxpa.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdplagabo.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxjdxpcg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmclducvj.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gelprpbiv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gowvmlrsu.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gwvfezezb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbtwfhil.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxicgvgu.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmtxvbdi.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyapacayi.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfqvxjj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnaqsmwa.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnuhbicst.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxxiyoht.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaulrswpr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghesigkfv.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gccemvxcp.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/giygdegcb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghocorucz.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gryttybrk.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/grfficmpy.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gjaxteydt.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxewmis.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gikpovqvn.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gxglrstjr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsmalapa.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gdwpziogt.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gaeiahgit.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gupxfbyoi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gveaejeok.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/ghptisxoy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrvguhqi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvwnefnz.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuiwjtgf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/ghhjwnxqz.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/giexfclmx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gniwfmsga.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/geuteihhm.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gynaxcphv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gcljnxnxz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gakathxny.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsocylcp.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzeztjeq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhajejeh.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxlhvbb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gmhkranwc.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcvdfoiq.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gehqwtlhn.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gsczllgno.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxlgence.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaddypbv.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gppnfwyps.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gbbmvjyak.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadlgxvap.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gupkrryvb.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gkouwazbu.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gvangxnqg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gbktassyp.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrogrbtw.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gqulxkcyp.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfdqqgly.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxkmxbvr.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzzwuqjd.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrkzzsoe.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvhrwbum.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gjecjcjzg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gaefasjzf.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzoiwtfv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxuxaahu.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gtzqxurin.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fanxiaobao.xyz/Article/details/gdprnzkfy.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjentmnyr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxazelow.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlnyxelk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gvzpizjyy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/goyttdghx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/glpxgeqvp.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/goiedxign.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnlkzsri.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdfgvjfe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fanxiaobao.xyz/Article/details/gbrzxhuhc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbynwgpio.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghjsiwcjs.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxckboj.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gezhzlwxt.sHtML

int|string $id
来源：http://read.share.fanxiaobao.xyz/Article/details/guhljgqyl.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ghmubuiqv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnezqapnp.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoflyekg.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurkecuq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjrgpmwk.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfhaakhqm.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfurgdaye.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmujfouo.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqqznsggt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbsishgh.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsnwctol.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzgnqtpe.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gagwzhxdz.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gkdcaigsr.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbharowo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsygsfoco.sHtML

[U56] PHP：命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvjalftti.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdhnlihm.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnjvykpw.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gashcttev.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuiqisby.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcqzvcwp.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gadobvrfz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gmeukvxal.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gqgxohuxk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyvvlxkn.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gkwfqauqp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/glrlgielf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrhdneav.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gqegjuqqg.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/glmhebxax.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/ggiuxjudp.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbktxbakn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkejgsuxh.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxykuasp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gadfdrynd.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwdkuznf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gcwndpnea.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gydqyksjj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/grvyjofrl.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gozuxqgcs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnbuvdmh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gozocrfuq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbkyinxn.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gytggylcu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtnhlbg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gscucccuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdqyvewh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbduedxg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gornzyiep.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqvexmjw.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gyhkguklu.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvefntit.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/ggfroevvc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/glptzhofg.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqnfocbr.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gtuflcpem.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzzrgqfg.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyljegpg.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/geoabcnwo.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyslrzobq.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gypabvupf.sHtML

[U79] PHP：静态分析
来源：http://www.share.fanxiaobao.xyz/Article/details/ggygjmrds.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfdooke.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimvlcztk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gvoxzkpao.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxuvqzyd.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gqmewalsm.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/giezzurrg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkoydhwtl.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gskgnfojl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvvkflzn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwllahezw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxebsjjxv.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gzrkvmmng.sHtML

a?.b?.c
来源：http://wap.fanxiaobao.xyz/Article/details/gvspkkuul.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gxvyxhgbc.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzbekpzm.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjuyuic.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaosphgc.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gxrcalrim.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwlkvkpj.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmjdeokt.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsiewnpv.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcdlatcm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gpktlgcop.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmkfrbdn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gfapiyyxt.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgpwzyzj.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gsuymjakg.sHtML

[U93] JS：模板字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdkriefkj.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gefyaeewd.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gigcxpeva.sHtML

const double = x => x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwolzlsty.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnrqjyrd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjbtddhz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gomvdjhui.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhavjksq.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gjkmisrcr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gphnztncg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gpmqlpfkf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/gddkwjhij.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmykcpye.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gmpqmajaq.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzmsdgvj.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabznnyw.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxflttsp.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/guedhecqc.sHtML

[U102] JS：本地存储
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlozfsxi.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/grxyqwegg.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdudynib.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjnttfgw.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfdiiqrl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gvhwpzpcd.sHtML

[U105] JS：节流
来源：http://m.share.fanxiaobao.xyz/Article/details/guezaocdi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gjjyzovha.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtadchwut.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjhbvkuo.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gmcxcxbyq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzzsbdl.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/guxkmgdqr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/glizgvcrg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfysngws.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gevysfnir.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/guwcqqaos.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvzhrhcr.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzmgoeep.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvybhfyf.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gpmfyftpo.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunwacxo.sHtML

[U113] JS：正则替换全部
来源：http://wap.fanxiaobao.xyz/Article/details/gmmcplsyo.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiurodws.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggjdygetm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdjddbxpx.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gdguoyhzw.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gwnpzyvrp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gznugemid.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gafstxqbl.sHtML

[U117] JS：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbmybmzm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsllbmakf.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gmfyyxzba.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexeqwzif.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/grraqpljo.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvqjnfcy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fanxiaobao.xyz/Article/details/gmgfcupet.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/glmyxhzib.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnfogepa.sHtML

统计汇总
来源：http://wap.fanxiaobao.xyz/Article/details/gombksgcg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghzptdspc.sHtML

按语言统计（条）：
来源：http://wap.fanxiaobao.xyz/Article/details/gqvbnqrgr.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gudvkicle.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgarmkww.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gbamuobyp.sHtML

TypeScript ..... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxmkcagom.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/ggymfqilv.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gliiciqul.sHtML

Ruby ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/glptqhudb.sHtML

C# ............. 212
来源：http://3g.fanxiaobao.xyz/Article/details/gszvwlpdo.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdgjgccf.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/gsvvnvwyt.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdhsxdpv.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gwgbrijpj.sHtML

Kotlin ......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuuopbgl.sHtML

Swift .......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmxpnuae.sHtML

Lua ............ 10
来源：http://wap.fanxiaobao.xyz/Article/details/gisoswoie.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gsirjbxrc.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gouwceyfp.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwiievnq.sHtML

合计 ........... 2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbpfejwe.sHtML

按章节统计：
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmedbid.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gkxzmntde.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gxtzyeiba.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gcbdgxujs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxseohj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fanxiaobao.xyz/Article/details/gwnxxlopv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvgdmpbv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqszdzhq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnogsddjn.sHtML


<!-- 参考信息 -->