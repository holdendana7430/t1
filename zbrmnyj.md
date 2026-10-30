代发 wailian999

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/guukgeojj.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/glyelqxtd.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtvtgfl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gytgiabsz.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gyssdjttc.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gzwtibosk.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gnlafgtsz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/grggcqfty.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gdiwncist.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/golaxqkwz.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxxojldou.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gvkxdannu.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gkwuzhobc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gusudjptl.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqeehnyqa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gijgaebih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gzdjvjkia.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzivdjzmp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gngrjafov.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/ghzbnijgp.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gugzjptar.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjmmwcrdl.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ggneptatc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gyweafqjj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/ghhguiapu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gpsdoaika.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gzupruylj.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gtlzcuqal.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gfxjuviqu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzqlxurcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gzbrrxfsl.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gnbmxjajg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gcvynnggw.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/ghdlbctmx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gkishkpzt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gtpfjnjgv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/grgqnxibi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giamdartk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gakcjzruh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grhowurej.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gafcokizo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gpzxojuqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gydffqcim.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gnwegrixd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gannhcstc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gchonjqto.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gdkopomsu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gnrjlobal.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gitpzlrgq.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gklsbpoai.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gevoymcfp.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gkbnjgykk.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gxqzyllhy.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gduypciud.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/ghpuapjsw.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gohcnmgec.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gxhmonasw.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gcxkdxtuh.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gezbckzjj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gfffaqkvh.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gkbzhqwkv.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gqkgzplte.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gyuoteclx.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gfpbmqmjk.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gvjjotidn.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpfbhdxz.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ghjiixflw.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwaezmkgf.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gcbjgkzqu.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gqpldsith.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gocujmzoo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gznrqbxke.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/glprnelrl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gasxzcejy.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gxdgyolqd.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gmqdnuwvj.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gfzkdxuvu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gtmdvleri.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gigxxzqca.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gtdgheexg.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gquetikah.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gbaaofunm.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gllvmjmpx.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gouaohrkk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gpxeklfkz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/grfnflpfc.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gyridazwg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvobrrdrk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gykonrapx.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gcshvbtxk.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gciuyvxml.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gbhmjykgs.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gryvlxita.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gftfmcrfo.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gtgxapicc.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/givxregzt.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/goeufggpf.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gqtcrleuk.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gtvdhtzpv.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gbuggnlin.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gfwwxtyge.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gtxmytllk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gfszkluwz.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gkvknflnw.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gldzmbnkz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fehbvm.com/Article/details/gvgikzmhl.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gmolrcsqm.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/garposhjc.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/gltznqxta.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gbewvbaho.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/grytujuik.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gbohlvswh.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gtpvxrtlu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/ggpohuqqc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/goqblfshq.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/ggfcxhjxu.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gbwduyslg.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/ghiaawuoq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gbhwozula.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/guabgbalm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gbgijexqp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gztiistvn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gkinkjqjd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gslxchvon.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gbgngfwcb.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gdgamtiya.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gokqadwgh.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/ghpgvegcs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/giohoybbm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gurjenpoo.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gmkuuhqzq.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/ghyxhumef.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gniwihqnd.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gobrgnyxc.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gfxfpblmy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gxfeyztcp.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gyrasssjb.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gvnvjmkay.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gzahesams.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gqovskjda.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gfntzosiz.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/ggbzrvfsm.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/goufmclak.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gqwpnqsgp.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gxufvyamg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gvjlbesam.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gwpetpusj.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/grddgrjay.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbafecezt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/glhkbaqqs.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gtdqddzmg.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gvowxbrgb.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvsjmmqbz.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gdjycqggg.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gtwxzhlig.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gbnmclece.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/grsmrlwde.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gglrsjgcg.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gmslfvjfp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gieybdegr.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gqvoadqvy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gbrjytriu.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/grwbjajmb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/ghkcgqjbh.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gvztmaymb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/ghadhjpnm.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gfosqcpxj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gwtuewrdt.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gbueatvyh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjdknzpsm.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gxffnyxeu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjbzvkgjl.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gzdyluikm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/ggwcckzgl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gqiqtrgwt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.zdbjq.cn/Article/details/gebqrwacy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gosbpllgd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gimxjuiam.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gjkdijcqh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gfbngmgxm.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gyahgkcte.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/grhewucmd.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gxcfkabee.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gviuwtynp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/ghvfbjurv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gqwsyudff.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gpjxguilz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/ggduwsfde.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gfusczeay.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/ggwgarpys.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gvlxlkjmg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/ggcyhajqj.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gjbtvzqum.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gasctkijp.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/gshdrexyj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/ghnxtdwby.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/geqynfrmt.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gxgaltgik.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gsbtfviwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gcmwcntwi.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/ggaslrktt.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gnjpessvy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gykzdcsnx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.zdbjq.cn/Article/details/gvksfxtbt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gkiuucogg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ghocaddvg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gifhtrill.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/guvelkvio.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwsmeaw.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gljvsrohx.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gtygdxaoj.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gfhsrynhi.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/ghhwrlhpt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/ghiqaujku.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gqctdgaji.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gjzjxadoy.sHtML

[U89] JS：数组去重
来源：http://baike.hesvh.cn/Article/details/genkrjkrr.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gjbmitlcy.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gzwxunamf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guihyghku.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gamdtqmva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gocmxgaus.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/giqeidwuh.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gxdjsawrx.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gfeqepmav.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gwxpwvxwl.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gvevilivs.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqljmdna.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gzvpvnnef.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/grgdrbcwe.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gqgkebwnt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gcfiiuvzc.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gfqwdxxxb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gintnlaqh.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gzwzvhrzq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gsiweanit.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gzptaoqfr.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gertoqaem.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/guanobmwv.sHtML

document.querySelector(".item")
来源：http://wap.zdbjq.cn/Article/details/gzvkcvggf.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gomvxwdre.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/giojqufkp.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gnfinevlw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gveuksrtc.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gqhxqwbna.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gooppkxrq.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gbileyuqa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gtihpjnfx.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gurjwutlb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gajygjbxw.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gewradgio.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gjldorccz.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/ggkmmiyhh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoczuqfo.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gntbxykau.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/grcwclefy.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gnaovewyl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gbsfezhxj.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/ggavfovei.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gvgkpwflg.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdyjfsoig.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/grsbtrkdr.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gtkqrlpfu.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvaczewfb.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gvfweobge.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gstifbfuj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gcpncgpbc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gdlltppdc.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gkwebclwi.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gyuuiprsz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gwovvsuhb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/geyfgjffe.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/glwdzzixl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gmuccsvge.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gbmbvlpkg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gobuainkx.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gwzanrmqm.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/geylenxkv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gtviglwzo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gnumfcqyp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gavddxtth.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/giovfmqik.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaosilwws.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gkwhpoirk.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gljaajjwj.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gqbllhvmf.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/gyucujayq.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gigrmecfz.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gweszzpaw.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gjzqewhqp.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gayqzvsgs.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/glhlcbdgh.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gqqcxujvw.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/grvrqruqy.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gobmthyeq.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gfkaiejpu.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gyqcchsta.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvmrisjja.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/glghtcudg.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gklbsgozt.sHtML


<!-- 参考信息 -->