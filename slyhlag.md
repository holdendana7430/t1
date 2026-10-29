代发 wailian999

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmdncqenh.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/ggvauwstg.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gcylykbma.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gomizxpcc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gddcimrei.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/grxzlfdrp.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gnsxwfssp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gmtujlmou.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gwzvppjia.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gibiugfcm.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/goaqzimsn.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gzbtnrbmo.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gpzbolpel.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfyvvhfwi.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvtimpnjf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gxqynzuyf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gwzvrrtyv.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gbephfwyy.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/ghabgmiii.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gvqyxrhui.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/guwomzfrm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnafrjvmw.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gcghlelhf.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gmztgsgmg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gfmuupnwj.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbgzkcpon.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gghazvugu.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gnhucclhg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gryuaogjx.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gbmeccylq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gfwfmerkx.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gjhlgnvan.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/goedlegec.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gyebpgxsi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gudngmgtb.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gkxbrpdhs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/givdbmhry.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvouelfxm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gljrfhosi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggfvllduo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/glqmpnvxy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gotqlbmer.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gpgbksocy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gqyovohzc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gcijpgqkx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gkdbtxvbi.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gvnfhiisg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/godtkaezw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gelroyhok.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gbvycirhb.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gcyvvvkct.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/ghhbfqzzw.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gvomftogc.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gotutrxbf.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gcahlpgyd.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gvqssbvpm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/ggfsrsiut.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gmlpkdvxv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/goywyaaov.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gipwxvuex.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gjaipnpot.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gebhihwvr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/guefoihfz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gmfukwzew.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/glifqhrgy.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gbknrsxmw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gkwazizxk.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gwytthckl.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gpxujffve.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/grntqrrwc.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gvaacemnn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gsojmjsxd.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gxsephwzj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/ggpwdlpzr.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gqrjmbmxy.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gliukdrzj.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gzlkqleji.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/grcoleshc.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gphdhdkpm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gatljulfx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gzteveyaw.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gjegiquit.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gbpxqftkj.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/ghezocfvw.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gkeqmkynp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gogqemunr.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/grtghspcc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/ggfzrmsvz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gkpjylbgg.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gyuipipsl.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gupyklotr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ghegxkmjl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gucvlrbtg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gpkdkfeeq.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gocnrcruv.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gaqpxfazp.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gbxruvrzb.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gmtemirrf.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/glrxkgdve.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gxapjwytn.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gwtdehxov.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gqbzfjctj.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gksugfexi.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gdwvwnyak.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gchnetkub.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gsqbtslve.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gekrhmiyt.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gjjecdzim.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gotiwoeur.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gzwwxcrlo.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gzgeailqv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/goywegaeg.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gncwxrocx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gzbwpmacv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gfqyuzbrg.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gsnvtpzin.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gfbuojhuo.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/grvzxwuap.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gomlkrqrl.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gmewsfheq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gzhjkjmxn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gitbvlkex.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gezkughmn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gprngindx.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gpdxyledv.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gqmabsoyv.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/grzalfjgy.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gfarlepde.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gyvqljkhj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkffwqcxv.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gbbndgudf.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/ggbhrwful.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gjhekrzcd.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gspnxsvjf.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gusbsozsx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gvevpgxne.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gwvvrwssr.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/ghaehnolj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gdxrsfeke.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gfntzdxgq.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/genwhppft.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gqcclnpbz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/govcndgns.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gzwdtdstr.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gqujzxtdd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gtcsisyee.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gwusplchk.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gryeuffuh.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gfybfoxfk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gaembgwmp.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/ggzzjemiw.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gjdloolaj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gqcihvbva.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/grgyundlw.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/glbkcpfsl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gkqqfqxny.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gtjwdsnva.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gqnfkrijg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gthcjtjzx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gmpzcuabc.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gnmyjhrmb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/glssuenjy.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gryfoeftr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/ghhlhwdjc.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/ggqxjvxsp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gdtgspmru.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gffljjwba.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gxeimwzsi.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/guotnopdn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/getxlqatk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gcuiymmiy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/ggpupdliq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gyiedxzsz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gwmsjfayw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gkknrrfiy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/gtqlftucq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gatzqmciy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gtsqefwvg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/grcblqjww.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gddrlpiek.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/grasurnfz.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gykkpujnn.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gjycsprfd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gwmczyiec.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gmceqtboo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/ggwitmkpa.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/glvabskkj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gklbelmfo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/ggssuycrb.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gvhwfstye.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/godkpwwix.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gpvprciut.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gtoaozmbf.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gizxprbwp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gdtrcpfvc.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/grqyxoefy.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/ghsdqptqa.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdvydiu.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gsssejgxz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gcepmseud.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gmnjshvhx.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/guqdymmrf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gxrpurrik.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gjjwcfgcf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gyiuogmtu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/ghiqhsjew.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/ghkncydxq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gymtpnajx.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gyyxwvxzj.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gwlwodqqe.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gxytlmulp.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/ggwxvtrob.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gevwggqfm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/ggginbgpc.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/ggdqgxqyz.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gujeyrquj.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gavgxvprv.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gdstxnuhq.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gupjkyaij.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/geymvwqgr.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gicmkksln.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gagcfubhk.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gbnrsrwlz.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gyvracijs.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gurcxoaiu.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gxwpgglli.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gshjgvbwm.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gwhptibig.sHtML

[U95] JS：Promise 包装
来源：http://wap.zdbjq.cn/Article/details/gjkygzryr.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gpachmmlc.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/grnmqssjs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/glvfobpvt.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gujfnveyi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzfrzxuzw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gsrabqdgb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gyfxjhdfb.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gwmgynyjh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gneesjnwj.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gdgnsiqkv.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gvnxrcpkt.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/ggivofskk.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gypdggqfq.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gwjfjyezp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gvtpsmtov.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/gifxbajov.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gsdtaesht.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/ghluhsmsq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gjytwynrg.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gsbdyvlci.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gvgjzamrw.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gltxnscst.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gvoyeifmt.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/ghgqdtpmf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gdnhlputu.sHtML

[U108] JS：随机整数
来源：http://baike.hesvh.cn/Article/details/gboxhqley.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gpvfbzvzz.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gpxpfewmb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gdproojyk.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gfdtuhddt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gquyfdvjr.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gfhreispu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/genixmike.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gfbkazrrg.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ghzcfujfv.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/glebihomt.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggdqggbik.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gerolwxqq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gwphxictp.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/ggcifoase.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ggirbhuul.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/ggoqjdshm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/gzxlruvag.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gtbyiwksj.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/ggbhoprqu.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/grtctlsua.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gvlnasmqd.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gzhwpnbkj.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/gzwtyuujd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gaqtjjamh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gelbyvltn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwxemwcpw.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gjstuemar.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghtvovduk.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrzuzdk.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gwbcfeezn.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gbinclymv.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gzdewepua.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/ggerdqlrj.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/gnmswiyfg.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gchxqnpup.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gwmekyfdp.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gtcelpkva.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gnubkvoqv.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gkdypubkq.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gabmjfasg.sHtML

Bash ........... 80
来源：http://wap.fehbvm.com/Article/details/gyzgzwemj.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gyseigwbq.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gwfaksmqe.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gzdxkcsla.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gyjqgmcqo.sHtML


<!-- 参考信息 -->