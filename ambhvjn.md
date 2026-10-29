代发 wailian999

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gyhnicxsi.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gmyjxlrjt.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/grqrsmspb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gunorgxix.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gpwxgmxcz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gqhiyondh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghyufspmx.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gtjmcobne.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrtneeau.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gidpixxwo.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gvmtwfsdv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gfsycpygo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gkzcmkwag.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gigiqkwdg.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/ggjppihnh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gvchyooms.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gaelaovhb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxzmowukl.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/geyggzljy.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gwbpvnkxj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gazzbnokt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gewedutcm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gisunmfxh.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gyjytfuzp.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gjflpshto.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghftdeclc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/ggkibuveb.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/giyusjieq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/giytjaach.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gsqbpnqwz.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gffrbxthz.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gsgmfkkpo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gbgpygglk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/getavowhs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gwnuyvezs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqocaxheo.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gplkrkljl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gjeqyvwuo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gnuuodudn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gdnqwlslc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gtgqbzmrq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gicqlvhzr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gzmfaicby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gxbrvzyez.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/ghmfhjnos.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/geikgrusj.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gufeyxusj.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gidnvnbux.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gwrwhpnmq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/ggmuhmxhu.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gkvnljjsu.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gwvdbkyry.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gvbzlnuyx.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gbuxagspk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gwglxkklw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/geiyvyyfk.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gvogxwcqw.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gmyvpeiiz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gpszknhns.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gygwjydex.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gkezhcfhr.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gmktdrlke.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/ganzkcygt.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gypmfnvaa.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gypprewwg.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gilkijsws.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gntelhenr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gaecrjqsa.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gvkzjqibp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gopclqvmw.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gbbukqvys.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/glibnucjo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gdkpovddh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gbbameeic.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gpmyyjkqt.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gtqqqaxtn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqseqhrxv.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gbtizshyi.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gzdzmzoew.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfrguql.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gmeatcngd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gwjqkwdrk.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gmrwunhht.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grxizpdde.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fehbvm.com/Article/details/gppbpcwyv.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gzxafkiaz.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gwouainfe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gebucryff.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gboripbua.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gsbwijeyr.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gxchhzqej.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/goekjnytq.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gxtluavku.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gikbbowqr.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gcnlnzfax.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/guwusvieb.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gjzcwniwr.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/guxoiffzl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gkekpawiy.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gkhypezlh.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gnaazlkbq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gjtixrndp.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gqiovziwd.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/ghmgwnkcx.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gmvynwpcp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gecpzdsra.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gfwspmwgf.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/ggcbtsinq.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gtrdghrhd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gdyhfbsxz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gcpwaqsxo.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gknurgekl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/grmcrytki.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gtzmzlbqp.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gsmpspspd.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gamhhrplj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gaejsclgm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gqvqytnes.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gyggavnmu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gferzssaq.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/givnbklmg.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gsbwvcemw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/giogngsqv.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gsimnyjzb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gyiszgpgq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gpuvkqszj.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gyuprgikk.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/ggukmlllq.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gmzyfadsx.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gvfvbaosh.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gjulgfqri.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gpuqgjpvm.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gusyymhkk.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/gxbjoquvz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gcquaqglq.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/geyjymywu.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gqxaipuqm.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gjsmjsvnj.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gwnvohbfl.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gyngduuzt.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gaauisckx.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gqwavmtfm.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gjqfzreyu.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gdbggmstp.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gddzoputj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gnuefdber.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gtmijwjnf.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gyfhldkwp.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ggrpqcnor.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gymsigiju.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gpcwuucxo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsfjjyvzf.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gknksyurx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/glljbgqmi.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/ggnfoegxy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gummjdokh.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gebhsvxys.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gzzvwbnaz.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gflarrxze.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gxwpzknhg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gyaenxqnd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gsnasdwmy.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gstofghgm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gpsasemop.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/ggkyuburt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpdwgqfxz.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gabelxhax.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gyuwypcpy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gsyxkunff.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gminrkeoc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/ggkdaezzd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gihutsizn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gbboxjltn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gaeztoefl.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gtqvyfube.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gfawbsmrt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gbnkbouvc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gzrljbtos.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gummfjnjm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gdbacbgwv.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gdiliikyl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gcgdijyiw.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwnmxvobb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gaxmdiltp.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gjfpthnaj.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gepkfhakp.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gtivztotf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gvreubnqj.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gmtrtajlh.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/ggqzdpeaz.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gmgozwolu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/ghjhmfkyb.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gewkdqydj.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gpbrhcsyx.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gbkzeuibl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gnensgtfp.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gekmplbwr.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/ggvglzctj.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gdlbmnmah.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gvxybdihy.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/ghyzatftb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gqfzdnwrb.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gagidwnje.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gqvvtgqgj.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/girtnyfxd.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gdwcmqlnq.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gmrvthxlq.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gacvwwwdo.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/ghphnxndd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gccklzexa.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gzsveebib.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/girsrjohw.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/guvpfpzeh.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gaqelqmmm.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gurwpbejp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtefvgnwb.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/gmtpjsmsl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ghlyiswsz.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/ghvmirxkk.sHtML

structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkzlvljsq.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gyqgsogup.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gqbqexdcu.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gqzymtyqs.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/givxaoanx.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/grzvkbhxs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/gedrurewq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gttjnguzq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gozdxqoix.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gbxxwuupd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwlaurbhx.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gixlxooib.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gigkcqbmv.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/gkgwcqkfb.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gvmmoavko.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/grvvgabfv.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gtbmfuogm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gzfpuabhq.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gxomlarnk.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gefuioxfz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gqpxfidrn.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gclbepnnb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gpdldxcsy.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gwynskeno.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glnypzhas.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gphmcjbvs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gntpllgxv.sHtML

[U106] JS：日期格式化
来源：http://wap.fehbvm.com/Article/details/gspbtlhic.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gvqarblpc.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/geedrxtjl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gadqbuwmo.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/ggcakkoui.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/guhdjksgc.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gykczlfok.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gjswojnrr.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/grkyxgguk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gxwdaclrp.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gtscmptew.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gjgltqons.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/gssiobnbd.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/glhnsqmbl.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/glmgsywmj.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/giwjmfcoj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/ggnddxeem.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gebmbgmoj.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfxgeufov.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gurwbrxdp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gagyobixd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gruouqyia.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gihhnchkv.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gszgwovht.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gkfbozake.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gnrcecomd.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gvgizrjvx.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gkmjwsril.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gjbnuregc.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gdiiwzjjx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxaqsueze.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/gpttdznpz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glrvhchcw.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gbdvwtrji.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gyyocnpya.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gwtlldfcu.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/glxnsquiq.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gjjzlflvb.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gigbxrxvm.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/ggekxgwko.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gipsryuiw.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gyldsvyvx.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gtkniagud.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gppveifdd.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gcjltzsis.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gdiwpensg.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gdtcpwmve.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gadmqlmar.sHtML

Lua ............ 10
来源：http://www.blog.fehbvm.com/Article/details/gyizvfopn.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gqylvaeax.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gocffqpar.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glgqpnytx.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gthsmaiqf.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gfkxrsshm.sHtML


<!-- 参考信息 -->