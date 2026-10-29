代发 wailian999

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gafabsfdu.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gkgoyzuzz.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gaenmzokd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gsfqdvlqe.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtafvbuzj.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gfvzkaggy.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gqexeiaak.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gqzmbzqvd.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gvkmeuiyw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gajlzygyb.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gagqorgkq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gedrsiijc.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gcfovkawy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gknsythqa.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gnzhwdyqp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gkeywgpej.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gsbediejb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gqrujuins.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyzesynam.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gcgejcyad.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gxlubaklx.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gngaizggm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtqtgjejm.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gcotzbqsl.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gpbtmmhva.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gheotehhp.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqdtucdry.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gzevcnjwb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyjowiphm.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/grdnkgurz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmapxblnn.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gvdnofynw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gwwlnruaf.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gbhqlioxg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gudpwmkmz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gceefpepz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gorulmlis.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gmbsgaixs.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gfswbopyx.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/ghyaihlfc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/godasqria.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyegxlitd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gmwnlpodc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwajvcifs.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gndzulhpb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gutrbaudb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gjlbenvia.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gfehrwgjv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gymvujpwe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/grvipqmkg.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gzevuancb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/ggbaygkfc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gimrqyyof.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gwvdyvssr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gyqswzfox.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gcfntbvoe.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gnddjsqcq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/grmzcjrwh.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gvrqxucuv.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gtfzcvkjt.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gkfeqzerf.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmbvoxc.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gixvfrzcb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gwobsuwgo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gtudxbjpj.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gcdxwucrh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gmhcjrpdy.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gcaaroxll.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gysckzqnn.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/grbbtlbtq.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gzjiaxebh.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghokemebw.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gvzacjtkh.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gkdyfmjsi.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gprboyerh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gcqxdrgyl.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gfqurvcop.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gqejnoebu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/grpgwrenb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gblwlrmlu.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ghgfeblbr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gjhfrsodq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gwbwbhzyn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gyshwwshx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/grvnxvknz.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gfucxtzwg.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gxevwhnzd.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/ghtokslky.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gmvkwhrnz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gkvuegwtn.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gnrihohbm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gjgiwkacl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gwrkcvhtl.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gorfhvbzp.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gsgcejdck.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gfvjqsmbd.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gwmgnnjwt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gtltwrrcy.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gvgyqqtgt.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gdmxovnar.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gxazourpm.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/grulmantt.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/goagelvjm.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/guptrkern.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gkuijojoj.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/glfiyxbaf.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gtaatofpf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gwiptszqw.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gaozkzxsj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gxepieyqd.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gqszduaws.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gqrugrkgi.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gdnlgoumt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/glcwwskwt.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gyjpcpwhp.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/gzefoyenw.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gqypysckg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gmbjzuojw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/ghxkttlrj.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gawlaozdl.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gzvmexfvg.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/guldgqriq.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gxejjyonm.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gpjizbvry.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gefxaqwop.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gkaujhpnu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gckezgnlw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gvkrgwcue.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/gianqjorx.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gwzoeijvk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpgpcir.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gmfolqjzn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gttezpxrc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqsuysuoa.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/giwdbhgtk.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gidlyetcg.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gziqytzhm.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/ghdsagjti.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gahicsizb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gspeesfdi.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/glzozctmp.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gjyrmbmrq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gmmavdxjs.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gxlzeckby.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gmhduvfmk.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gddwrjjyo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gbzbflkqa.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gifaqtvih.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/goyhpcxsc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gajqpesbz.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gjweemyqn.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/ggeazxzcn.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gqxdjrpbw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/ggtmqryla.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gzzysnkta.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjlwwxbfb.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbulbovii.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gcgffhmez.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gihngcxdb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gcqqedytp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gfowajtoi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gqtgursqw.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gkwdhaaep.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gomktolgj.sHtML

[U61] PHP：正则
来源：http://www.blog.hesvh.cn/Article/details/glwgmjriw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gmwglbbkz.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gfxivujrp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gopzsttfv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gojjvcpmw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gbqueneyl.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/ggdcabxwo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gyxvmpmim.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gexxzxroq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gqutvzxwq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gjqsushov.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gnceaktac.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gftdsuxvc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gquusfbvk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gqgywtgxc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gvhheauwu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gzrlduucg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gornmyweb.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gewwsolyu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gbnyyqrjr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gbqrzldse.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gamylahsq.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gpdiintba.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gylxofbin.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gddeqkkak.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gkfzkhxsa.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/goccpeksr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gzjmfueuf.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gzcpibhaz.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gawlpsdvg.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gqbayoizk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/geophjjcd.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gvtxpfoys.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gqsdgbvgi.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gtuupgtqx.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/grmikvovx.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gbllunrua.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/ghybaqxem.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/ggqsvakgp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gvbfnmxfe.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gqoqvnreh.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gldmcrkpo.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gygcfsolr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gbytyzccc.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gmutnosnr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/giicyaehr.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gdusfsoqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gwwnkjzdx.sHtML

[U85] JS：可选链
来源：http://blog.fehbvm.com/Article/details/gczuliyfq.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gedtcfsdm.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gfgyhxckj.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/ghncidtum.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gkrhtwupw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gusmfiour.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gxaxcvucu.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gzvnmnuev.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gkaikfetg.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gqbzrvmrt.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gjpfnvdlb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gyfrfxtsq.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/giyosnepb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gpvnasbhx.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gbsnuyezg.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gxeglnbpu.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gxtrmghds.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gmrkzepqu.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gsijftden.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grinmfqbz.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/grfxvynft.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gakcahjor.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gzkzsyeyj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gjowtwxnk.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gyvmcgcrb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gltmkbric.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gbnoqxztq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gvzfvddhy.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gylfqjhvu.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gnbspjxjj.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/grqkylipf.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gyhfbvenm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gvrrkwkah.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/guzpsixex.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gshcilkzr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gibnvnxdy.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gzoaefxal.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gnscmpzrk.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gswjdqkez.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gnclfqcvw.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gvydplflx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gbpbeonma.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gjtytlbcz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gxxrxggdg.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/getjbukzd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gbuxitlvl.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gfdpeeqcw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gbyjzymmi.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gsnybftdp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gcbcxhopd.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gxmbifgxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/grxabpiik.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gdzntemmk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gypgbxinr.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gioysprdx.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxwyfgq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gsuzwehlx.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcsecfgfj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gmkswvmis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gtqpqxfco.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gpgkrxafl.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gfqnebdlw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gojgxhlpy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gfwomriry.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/gefirsugj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gqwfhswbt.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gssosihuh.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gtawtfgfd.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gifgwojlg.sHtML

npx vite build
来源：http://mobile.hesvh.cn/Article/details/gpqgzrzad.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gkehfjsly.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gfjfsksre.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyuzmnpar.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gcjjgavhl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwnzalmtp.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gtrflkorx.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gdzomgams.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gxbbearaf.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/glbjigviv.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/guczhjamt.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gumycwjtt.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gnzgyehoz.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gxfztbfyn.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gzqrtfabm.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gwjplwlvo.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gmcdmqjyh.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gemnlzqxb.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/guektrqcr.sHtML


<!-- 参考信息 -->