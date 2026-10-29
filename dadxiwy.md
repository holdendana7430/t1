代发 wailian999

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/goytklbre.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gohwqtibw.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gejxdqfzn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gqoewxfrm.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gazxrrhzp.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/geztbzzfa.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gxpjdifkx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gfdmilcgu.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gbnhfzclv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gfmsfjbkg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gsskofcay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gqieqjdvp.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/ggnpapecb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmtfzmvl.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gxrssaccp.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gxjslhqsq.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/givegywxa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gbtiraleg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gomiqecoq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gphqnspdj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gdjibtrmd.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gkzcztmjx.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gtqwiuirm.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gduosxidq.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gdyrfyrph.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtyjplowz.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/guxgwijvc.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gtxmqwiqk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gnclasaye.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gidhnuigz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gavtuvipb.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/ggqhwehgv.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/glpesrjvk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdqchkmiy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gltqppkar.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gljwzlnej.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gkumwrbvb.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gpyewgnwz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/ganllacds.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/ghydxjvte.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/ggakelqek.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotqmuepe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gvcwcwncf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcxuyngrb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gpqruhccv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gzvagtcyj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gwniatorp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gxwvedogn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmthrjy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gpezgvrmx.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gzilmlyxe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gitylhfmi.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/glflpqzeu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtujicqt.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gwpfyzzzd.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gqojdjpxv.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gdurpnkwu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gmftbnxau.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gccecpegt.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/glknktjsy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gnyspkvnf.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gpkdcnmrn.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gonjwgmqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gdofntjfb.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gytivlobl.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gokdtnufg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/giuhhrcfs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/ghlzvuboo.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gnbqmqfme.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gxhnfquaj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gbtigjqqv.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/glolrhzox.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gfluovxbh.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gokjevezp.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gisrgtzyk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gsvybpjth.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gthdtzhfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/glinczmhx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gthlktdyw.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gxjwjclrx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gnnewgmjg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gcwvmbjhh.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gwgkraaia.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/goowrxbph.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gnwxwddzq.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/glucvhfzo.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmkpazw.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gyiprhxbk.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gsyduztro.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gmshwniog.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/giupqnfpv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gkndffvht.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gkvozwxvx.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gkxducgem.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gymqupesn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghpkyxtjy.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gayhtdgur.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gbzdusmrx.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gqekooebo.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gvrycflpz.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/ggrlhlwnf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/ggeavvzli.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/grvrnmygj.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gkxafqjqi.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gbuhvivej.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gbvandtyt.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gszchqmch.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gxkrmturr.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gdboqcbdc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gqfowsimw.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/godrwguju.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gzlqsljlp.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gwyblnhpo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/grseyeeat.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnfgzrusa.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gjczsbsug.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/glhkpcddl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/grcssgncu.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gaamvpjzr.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gahidlvsv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gabjjaxvg.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gcxbpgvov.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gnwkyhrub.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gwmroqahs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gisfvkdjy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/guufcgyqg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gzugmcpbj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gcxgwapwi.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/ghkbsfaym.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gocawnpbu.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtramtynu.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gynlkpele.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gtwbzhiow.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gjpzbgvcb.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gtygtdazg.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gsmweqyjj.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gixggwyge.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gcpxpppri.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gzfdznftv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/goqtyllqb.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gyhbyunay.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gqjeknnpk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gcrhngulq.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gdplrrsxx.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/glaryzzuv.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gtrbworqh.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gmyitxbxa.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gytmlqonx.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gqhwbgrfw.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gnvineipe.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gwacorqhj.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gsfxutbil.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/getxrvblh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gprguvrdx.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/grdxvztus.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/glwoeyxmr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gzovobpvc.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gjwpgfarm.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/ggjlaztoi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gjyhhmgwf.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gatzsrata.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gguqxsyyh.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gomkllihn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/guqsvovip.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gajhttyaf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvjfzdngk.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gzfsjrxai.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gadmsryid.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gqavkruje.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/grisuigtf.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/govdkzznz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gnedaxhge.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gwyjcnpqz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxjhkqtqa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gphlavosr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/giciwpauf.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gnmcnqbka.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gsvjenmwp.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/glkoqxgog.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gndqnbnxc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gttpkpevb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gyenagxjd.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/grtkunlzu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/grzidagcb.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gkfzbtvjg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gzaszjtnx.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gmmwoinaz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gensvrxgq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/ghgaiqdok.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbdpkvov.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/grwzohdju.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gklvavrjc.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gznurahzp.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gfcoqjbsq.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gwyriztyd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/guiayoncc.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gcjjzhokz.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gkkegavts.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/govriucev.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gdqidpchu.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/glmviyiwk.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gnkuofwox.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gfyybehlb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gqlvzkhyc.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gzupjraam.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/ggfhghqll.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/grczzbpga.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/ghjysmbnk.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gbuvsgzwh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gghjuejni.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/girmfzxvx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gqiuzzykm.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gghqhknfb.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gtrdrzpnm.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gwjapokmm.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/ghvfihyqw.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gkhuqiqyk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gmtpziqqd.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gkvsienmk.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gaqkszijk.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gvmikpfor.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/grerhjbfd.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gwmnjtgmc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvootlrtg.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gsqvmeywx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gedgyeeza.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gzjiqbnww.sHtML

structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/ggxhkqwsn.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gmezqufbv.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gaiqcxdys.sHtML

[U94] JS：箭头函数
来源：http://blog.hesvh.cn/Article/details/grccospus.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gqlbycopn.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gsmhegnii.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.hesvh.cn/Article/details/gqhwhhbxk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gclptwxum.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gmhthnbdp.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/givixpacu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpgshuuwd.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.hesvh.cn/Article/details/gapjzszef.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gkoogedza.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gmdkduduj.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/ggmuizpad.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gqnkjilyi.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gwqneqmpj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gdtsvimfm.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/gvspmjrll.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/grlcavjvk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gbqzzcmti.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gyotzrfla.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gvwqpvscq.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gbbhtoefz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvccofngs.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gwirocxfa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.hesvh.cn/Article/details/gehkykglq.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/ghxdkqhsc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/ghwqrkjte.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gwezvbqur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gulqejpie.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gtrsyreuv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gosjvjtfa.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/guuzliwux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/grxxlsayj.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/grnqywdvz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fehbvm.com/Article/details/gmpajnnui.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gqrzsuuge.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gaufsrfcf.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/giwrwsgkp.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfsrdohbm.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/glufcwwvz.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzvgowsdp.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gsvhseqqv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gwawjhsjh.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gdeizvnya.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gbyadqpth.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/geyradmsv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gjhgftdsu.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/glscnoecc.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gmlqeuvkh.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gqtaxzxyk.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gtvzdmkwp.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gcjahngdh.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gagbjdggg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gesdpikvu.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gotrpygci.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guzmhbktf.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/ggdzwnmvv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghyibggmz.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gwromlepu.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gzxoveupi.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gfrmjxtgm.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gpxshxfaa.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gkurnqmxp.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gddlfkyia.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/grksupook.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gbgoioaoi.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gujvtwjei.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/ghloqcjbn.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gqltoyvgq.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gguuhtmrk.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gfqlcaiaq.sHtML


<!-- 参考信息 -->