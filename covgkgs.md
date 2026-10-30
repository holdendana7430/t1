代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghlhwiuti.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncbbjdas.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/ghhoarayr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gejyrgict.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gpkxpcwtx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjtujlu.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/grnqgmmud.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gfnwausfx.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaarrozpq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzhgtjyf.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/giiepsytk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gimqokqri.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdufuituk.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeabclip.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwrnpdno.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggivuziuu.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjagmplz.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaxgftar.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutcdmwk.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gxjavzhzr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqohyytxo.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggljktzax.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/giabirpbm.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gwortfdho.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpoavhyi.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtswsihcd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkojvukrg.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlorlplc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gwbikuwnc.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasdhtvhg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnisgrmj.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gzadcwvgx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfbwglgd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzljvdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggylkistb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtabjyj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gsomxhjjn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/goltcpmnh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gpabdcfyi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdrqthbi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gdoyilsip.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gctunxhao.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqzyadh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwywwged.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/glphcdwic.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvoqycgd.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gndaseazc.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gggjwuppw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlgycxhx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfmazptd.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gomduwvgk.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmcwgvin.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjpxblmo.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqogpnjt.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gyapiawww.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/gglwfzdem.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcbvbnbw.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgvjuyzz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmivhajr.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpezkbam.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gzastunmv.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gumbqsbcz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/ggvgwwymg.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfnqegoz.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/geigpkmxn.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyroljglb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/giielhklg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwtsjsou.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgxpajrb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gkyvzffhx.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gjxoafqsj.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/giwmqlngw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gfukhcrac.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsckaxolm.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gjwpwdpxo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhwswkbu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdsclkzu.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkcshvuk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxfkazog.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/guyzobzxu.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpbkqctfn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gljlcajkm.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/ggcopbbcn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwvpazfa.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/grhwtxsjk.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghexrovg.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoqdlmpz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gwzvwzyza.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gsalhcltk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdspzmkmh.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gcekcaest.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmqecnbk.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gngmlpgqy.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/glryiqduo.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/guazvpinf.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ghlzmoxil.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gkwldwinl.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gclamuyll.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsufhjsuj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gbmakqjje.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/grgteapyo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknciutry.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcavozpw.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gulxkzxzg.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfcdoflr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbidrwqvd.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gztcsgvhz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvcijsra.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gacutkblv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gqathouff.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gasryhlbl.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfcjodex.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnrnkysx.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpublfol.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/guzafaixs.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjlmfiuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gvpwopwqy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gecgekbtd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkafxvccp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gllcieqqm.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjmgznltg.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gefymyhmx.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gtodxuaxo.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpdvkvuc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gostylash.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmbeqxjc.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gysfluqbq.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gkafuhxze.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/goxrjbjvh.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gltchskgy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcvhgcpv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/glwgugcna.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfettfgl.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gibpxwqge.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/grbdtuzwo.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkdyyeah.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gvieeubrp.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/guieqsqfi.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjnlnkki.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gpzgqsonp.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvchyexu.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gvwjmcnde.sHtML

[U54] PHP：空安全调用
来源：http://wap.fanxiaobao.xyz/Article/details/gusejxvbj.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksrecutt.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/giranksrk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldsxjupm.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvproah.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcmiljnst.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxljgtdi.sHtML

"值: {$a}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfemgvkw.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gukxrdnly.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbciiag.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfzmvssq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxciebqc.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gvsbsjyur.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpurrzpg.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goenegeox.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcspcicy.sHtML

[U62] PHP：日期对象
来源：http://www.share.fanxiaobao.xyz/Article/details/grhfjeyjt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoperkwd.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gkbrcplol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gekoxqiim.sHtML

[U64] PHP：目录遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfqdiiuax.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gvtrasaga.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqyxplt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfrskwna.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fanxiaobao.xyz/Article/details/gywectmeq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrhnabwx.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/goydkywxc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fanxiaobao.xyz/Article/details/gaodzmdor.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgrcjqwo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/gztwkcvhr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtovnckoa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqcjqsv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gnsrxfrzh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gcskieqiq.sHtML

[U71] PHP：抛出异常
来源：http://wap.fanxiaobao.xyz/Article/details/ghegogwlg.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/ggryaaeso.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmokddzzs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbhsncu.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gnznmyqud.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjpgynwv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grtgcfcmu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvbcukbp.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwbgsem.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gbqmeaszn.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhiraxuy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gbbwnwomt.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/glvzvyysv.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gxemhgztf.sHtML

[U78] PHP：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gssjnujzl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gcksijsqd.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gulzhthce.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fanxiaobao.xyz/Article/details/gyxqptspq.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gquewggfm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiwuhunk.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjuvoeqs.sHtML

npm init -y;  npm i express
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigeapmj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gdwvuiucz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gkhosuwmv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllycjasu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyauxfyar.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fanxiaobao.xyz/Article/details/guwoykgog.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmxwjtom.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcbspazn.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/gyblvueam.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqlcwfxgc.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gygsjcgjq.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gqydatelr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gvgdmxecj.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gxcwoymlg.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gasanipbe.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwxadvxx.sHtML

[...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gbilagboi.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkubkqkyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzkpezse.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/govsjbhkj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gxnhefmfc.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/grjgrntus.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwzowfvw.sHtML

[U93] JS：模板字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgwykbd.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbysezdc.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwaobggaf.sHtML

const double = x => x * 2;
来源：http://baike.fanxiaobao.xyz/Article/details/groygqhva.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbiqybui.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gwibfzdjd.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gngbewybb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlsxswek.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/glzxxsinq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzlmngnc.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjptpzff.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gmfeasjet.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gjfraiiwl.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gnzlvafjx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoxxyqsm.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gisavnswa.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtrflynsw.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzswaqiyp.sHtML

[U102] JS：本地存储
来源：http://mobile.fanxiaobao.xyz/Article/details/gixaopnhv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fanxiaobao.xyz/Article/details/gdnwcksxd.sHtML

[U103] JS：定时器
来源：http://mobile.fanxiaobao.xyz/Article/details/gmutiihvw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvdroxkw.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjteumlt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfahhxav.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gdjoqunym.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gmoimsfmj.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gfynhqybf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gxyuzivul.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoclqlbi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddubzkf.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfrxyoaz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gdifpkxve.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/geqdhnyxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjzqhrg.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbpcszex.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gquwuvamf.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuschrqw.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvzkmylj.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gyprsqwup.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gauojksgp.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/grdlbwxug.sHtML

s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gqnpadjja.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/geztrsnrc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gzqdbggnw.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/guejdgxpk.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gvtcgridg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gsvcyidhc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcxorlblz.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/ggxvctktl.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcfkfony.sHtML

[U118] JS：开发服务器
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpfpkeeu.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/gqpeulzij.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtefvvpw.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdgwueqj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjyqsjit.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxovbgdt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwfqnvxb.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcdnyfek.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glzpnfuov.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzpmzeq.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswlhkmkn.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gebjtqsnz.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gmiuswxuy.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunxetyn.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/giedrthhp.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnuwcgma.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihhgrxvm.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gksypwaca.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryrxbkmi.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gxywrluea.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gxorkxelj.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/galvaddcn.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gicvpcbxc.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gxftppkor.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gzwrwgjcv.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtxupvxy.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmsfzwni.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpcwuzjf.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjpixdme.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gualtqtef.sHtML


<!-- 参考信息 -->